# Next JS

## What is nextJS?
Next.js is a React framework for building full-stack web applications.

### Problems with react to create web apps
its not feasible to create a fully-featured application ready for production.
react is a library for building user interfaces.
you need to make decisions about other features such as routing, data fetching and more.

### Next js advantages
It uses React for building user interfaces
Provides additional features that enable you to build production-ready applications
These features include routing, optimized rendering, data fetching, bundling,
compiling, and more
You don't need to install additional packages as Next.js provides everything you
need
Opinions and conventions should be followed to implement these features

### Why learn Next.js?
Next.js simplifies the process of building production-ready web applications
1. Routing
2. API routes
3. Rendering
4. Data fetching
5. Styling
6. Optimization
7. Dev and prod build system

## How to install 
npx create-next-app@latest
npm run dev

### ESLint what is this
ESLint is used to perform static code analysis for JavaScript, finding and fixing problematic patterns and enforcing consistent coding styles and standards across a project

### code inside src directory 
https://nextjs.org/docs/app/api-reference/file-conventions/src-folder
if src folder is there, componets, lib folder can place there

### app router
newer version, old it was page router

### use Turbopack
Turbopack helps with that by addressing two major pain points: Build Time: If you've ever worked on a large Next. js application, you know how long it takes for Webpack to rebuild and reload your app. Turbopack's incremental build system can speed up development by compiling only the files that have changed

### customize the import alias
next.js, you can use import aliases to create shorter and more descriptive import paths for your modules. This can make your codebase cleaner and more maintainable, as it avoids long relative paths that might become cumbersome, especially in larger projects.
jsconfig.json or tsconfig.json

folder structure
next.config.ts - nextjs settings
tsconfig.json - typescript
eslint.config.mjs - ESLint
tailwind.config.ts - tailwind css
postcss.config.mjs - 
package-lock.json - consistent installation of dependences
next-env.d.ts - typescript declaration for nextjs
.next - 
public - static assets
src - 

### React server Components(RSC)
React Server Componets is a new architecture that was introduced by the React team and quickly adopted by Next.js
This architecture introduces a new approach to creating React componets by dividing them into two distinct types:
Server Componets
Client components

#### Server Components
By default, Next.js treats all components as Server Componets.
These components can perform server-side tasks like reading files or fetching data directly from a database.
The trade-off is that they cant use React hooks or handle user interactions.

#### Client Components
To create a Client component, you'll need to add the "user client" directive at the top of your component file.
While Client components cant perform sserver-side task like reading files, they can use hooks and handle user interactions.
Client components are the traditional React compinets you are already familiar with from previous varsions of React.

### Routing
Next.js has a file-system based routing system.
URLs you can access in your browser are determined by how you organize your files and folders in your code.

#### Routing conventions
All routes must live inside the app folder.
Route files must be named either page.js or page.tsx
Each folder represents a segment of the URL path.

#### Nested routes
[productid]
parameter will give 'productid'

#### Catch all URL segment
it will catch all the nested routes.
parameter is an array
[...slug]
[[...slug]]

#### not found
not-found.js file will take all the work
'notFound' default function also work

#### Private folders
A way to tell Next.js "hey, this folder is just internal stuff - dont include it in the routing system"
The folder and all its subfolders are excluded from routing.
Add an underscore at the start of the folder name.
_lib

private folder benifeats
Keeping your UI logic separate from routing logic.
Having a consistent way to organize internal files in your project.
Making it easier to group related files in your code editor.
Avoiding potential naming conflicts with future Next.js file naming conventions.

if you want _ in URL use "%5F"(URL encoded version of an underscore)

#### Route groups
lets us logically organize our routes and projects files without impacting the URL structure.
Wrap folder in paratasis (auth)

#### Layouts
Pages are route-specific UI componentsA layout is UI that is shared between multiple pages in your app.

Default export a React component from a layout.js or layout.tsx file.
That compinent takes a childeen prop, which Next.js will populate with your page content.


### Nested Layout


### Multiple route layoutes
wrap in the route groups


### Routing Metadata
The Metadata API in Next.js is a powerful feature that lets us define metadata for each page.
Metadata ensures our content looks great when its shared or indexed by search engines
Tow ways to handle metadata in layout.tsx or page.tsx file:
1. export a static metadata object.
2. export a dynamic generateMetadata function.

rules:
Both layout.js and page.js can export metadata. Layout metadata applies to all its pages, while page metadata is specific to that page.
Metadata follows a top-down order, starting from the root level.
When metadata exist in multiple places along a route, they merge together, with page metadata overriding layout metadata for matching properties.
its will not work in "use client" directive

### title metadata
their is an optional object metadata
title:{
    default:
    template:
    absolute:
}

## Navigation
### UI Navigation
<Link href="/blog></Link>

### params and searchParams
params is a promise that resolves to an object containg the dynamic route paramenters(like id)
searchParams is a promise that resolves to an object containing the query parameters(like filters and sorting)
while page.js has access to both params and searchParams, layout.js only has access to params

#### Navigate programmatically
router.push("/") // useRouter
router.replace("/")
router.forward("/")
router.back("/")

redirect("/")


### Template
Templates are similar to layouts in that they are also UI shared between multiple pages in your app.
Whenever a user navigates between routes sharing a template, you get a completely fresh start:
a new template component instance is mounted
DOM elements are recreated
state is cleared
effects are re-synchronized
create a template by exporting a default React component from a template.js or template.tsx file.
Like layouts, templates need to accept a children prop to render the nested route segments.


### loading.js
This file helps us create loading states that user see while waiting for content to load in a specific route segment.
The loading states appear instantly when navigating, letting users know that the application is responsive and actively loading content.

## error handling
### Error.js
it automatically wraps route segments and their nested childern in a React Error Boundary.
you can create custom error UIs for specific segment using the file-system hierarchy.
it isolates errors to affected segments while keeping the rest of your app funtional.
it enables you to attempt to recover from an error whithout requring a full page reload.

Erros always bubble up to find the closest parent error boundary(not in layout becuse of componet hierarchy(layout sits abouve the error boundary)).
An error.js file handles errors not just for its own folder, but for all the nested child segments below it too.
By strategically placing error.js files at different levels in your route folders, you can control exactlu how detailed your error handling gets.
where you put your error.js file makes a huge difference - it determines exactly which parts of your UI get affected when things go wrong.

#### global-error.js
if an error boundary cant catch errors in the layout.js file from the same segment, what about errors in the root layout?
it doesnt have a parent segement - how do we handle those errors?
Next.js provides a special file called global-error.js that goes in your root app directory.
This is your last line of defense when something goes catastrophically wrong at the highest level of your app.
it works only production version
requires html and body tags to be rendered.

#### component hierarchy
layout.js
template.js
error.js
loading.js
not-found.js
page.js

## Parallel Routes
Parallel routing is an advanced routing mechanism that lets us render multiple pages somultaneously within the same layout.

Parallel routes in Next.js are defined using a feature known as 'slots'
Slots help organize content in a modular way.
To create a slot, we use the '@folder' naming convention.
Each defined slot automatically becomes a prop in its corresponding layout.js file.

##### parallel routes use cases
Dashboards with multiple sections.
split-view interfaces.
multi-pane Layouts
complex admin interfaces

##### Parallel routes benefits
Parallel routes are great for splitting a layout into manageable slots.(especially when different teams work on different parts).
independent route handling
sub-navigating - When navigating throught the UI, Next.js keeps showing whatever was in the unmatched slots before, when page reload Next.js looks for a 'default.js' file in each unmatched slot.


## Intercepting routes
Intercepting routes is an advanced routing mechanism that allows you to load a route from another part of your application within the current layout.
its particularly useful when you want to displat new content while keeping your user in the same context.
(..)(..)foldername

## Route handlers
The app router lets you create custom request handlers for your routes using a feature calling route Handlers.
Unlike page routes, which give us HTML content, Route Handlers let us build RESTful endpoints with complete control over the response.
Think of it like building a Node + Express app.
There's no need to set up and configure a separate server.
Route Handlers are great when making external API requests as well.
For example, if you are building an app that needs to talk to third-party services, Route handlers run server-side, our sensitvie info like private keys stays secuew and never reaches the browser.
Route handlers are the equivalent of API routes in Page router.
Next.js supports GET,POST,PUT,PATCH,DELETE,HEAD and OPTIONS.

ex:
export async function GET() {
    return new Respose("Hello world");
}
file name should route.js

## Route handlers Handling request GET,POST...

## Headers in route handlers
HTTP headers represent the metadata associated with and API request and response.

### Request Headers
THese are sent by the client, such as a web browser, to the server. They contain essential information about the request, which helps the server understand and process it correctly.
'User-agent' which identifies the browser and operating system to the server.
'Accept' which indicates the content types like text, video, or image formats that the client can process.

### Response Headers
These are sent back from the server to the client. They provide information about the server and the data being sent in the response.
'Content-Type' header which indicates the media type of the reponse. It tells the client what the data type of the returned content is, such as text/html for HTML documents, application/json for JSON data, etc.

## Cookies in route handlers
Cookies are small pieces of data that a server sends to a users web browser.
The browser can store the cookies and send them to the same server with future requests.
Cookies serve three main purposes:
-managing sessions(like user logins and shopping carts)
-handling personalization (such as user preferences and themes)
-tracking (like recording and analyzing user behavior)

## Caching in route handlers
Route handlers are not cached by default but you can opt into caching when using the GET method.'Caching only works with GET methods.
Other HTTP methods like POST,PUT, or DELETE are never cached.
If you are using dynamic functions like headers() and cookies(), or working with the request object in your GET method, Caching wont be applied.


## Middleware
Middleware in Next.js is a powerful feature that lets you intercept and control the flow or requests and responses throughout your application.
It does this at a global level, significantly enhancing features like redirects, URL rewrites, authentication, headers, cookies and more.
Middleware lets you specify paths where it should be active.
Custom matcher config
Conditional statement

## Rendering
Rendering is the process of transforming the component code you write into user interfaces that users can see and interact with.
In Next.js the tricky part to building a performant application is figuring out when and where this transformation should happen
CSR(Client side rendering), SSG,SSR and RSCs


## RSC Rendering Lifecycle?
app router is build on RSC architeture

### Server rendering strategies
#### Static rendering
#### Dynamic rendering
#### streaming (suspense)

## generateStaticParams()

### server-only package
### client-only package

## context provider

## interleaving server and client components

## data loading
parallel and squential data fetching

## data mutation

## server actions
"use server"

#### useFormStatus hook
#### useOptimistic hook

## revalidatePath



hyration mening?

{usePathname}

##tutorial
file based routing

Layout

Template

<Image> - components for lazy loading
link vs a tag

usePathname()

react <suspense> lazy loading

reserved files

production mode and devleopment mode

dynamic meta data

app router and page router

pre rendering - server side(ssr), static site generation(ssg)

inbuild funtions - getStaticProps()(for ssg)
                   getServerSideProps()
                   getStaticPaths()

--------------------------------------

What is Next js
React framework
React framework
Additional features other than react are routing, optimizing, rendering, data fetching, bundling, compiling, and more
Next supports routing, API routes, rendering, data fetching, styling, optimization

Creating nextjs
Npx create-next-app@latest

Folder structure

Rsa react server components vs react client components 

Routing  and routing conventions (and layout file)
Dynamic routing
404 page —-  not-found.tsx
Private route or folder _
 Route groups ()
Layouts

Link navigation
Active link
Navigating programmatically

Template file
Loading file
Error handling

Component Hierarchy
layout.js
template.js
error.js
loading.js
not-found.js
page.js

@ naming convention

route.js

Thunder client extension


Csr,ssr(ssg),rsc
Hydration concept


-------

22:49