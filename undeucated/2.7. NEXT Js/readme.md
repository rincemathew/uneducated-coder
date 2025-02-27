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

### code inside src directory 

### app router

### use Turbopack

### customize the import alias

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