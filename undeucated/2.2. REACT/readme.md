


# React

## React Basics

1.  ### What is React?

    React is a popular JavaScript library for building user interfaces, particularly single-page applications where you need a fast and interactive user experience. It was developed by Facebook and is now maintained by Facebook and a community of individual developers and companies.

    React is a powerful library for building user interfaces with a component-based architecture, virtual DOM, and declarative programming style. Its performance benefits, strong community support, and flexibility make it a popular choice for developers looking to build modern, responsive web applications.

2. ### Key Features of React
    
    1.**Component-Based Architecture:** React allows you to build encapsulated components that manage their own state, and then compose them to make complex UIs. This modular approach helps in organizing the UI into smaller, reusable pieces.

    2.**Virtual DOM:** React uses a virtual DOM to improve performance. When the state of an object changes, React first updates the virtual DOM, which is a lightweight copy of the actual DOM. React then compares the virtual DOM with the actual DOM and only updates the parts that have changed, resulting in faster and more efficient updates.

    3.**Declarative:** React makes it easy to create interactive UIs with a declarative approach. You simply describe how your UI should look based on the current state, and React takes care of updating the UI when the state changes.

    4.**JSX (JavaScript XML):** React uses JSX, a syntax extension that allows you to write HTML-like code within JavaScript. This makes it easier to visualize the structure of your UI and keep the rendering logic closely tied to the UI structure.

    5.**Unidirectional Data Flow:** React enforces a unidirectional data flow, meaning data flows in one direction — from parent to child components. This makes the app easier to understand and debug.


3. ### Why Use React?
    1.**Performance:** The virtual DOM in React ensures that updates are efficient, making the UI more responsive. React only updates the parts of the DOM that have changed, rather than re-rendering the entire page.

    2.**Reusable Components:** React’s component-based architecture promotes reusability, making your code more modular and maintainable. You can build a library of components that can be reused across different parts of your application or even in different projects.

    3.**Developer Experience:** Tools like React Developer Tools for Chrome and Firefox, along with a vibrant ecosystem of libraries and extensions, enhance the developer experience. Features like hot reloading in development improve productivity by allowing developers to see changes in real-time without refreshing the browser.

    4.**Strong Community and Ecosystem:** React has a large and active community, which means there are plenty of resources, tutorials, and third-party libraries available. This makes it easier to find solutions to common problems and extend the capabilities of your application.

    5.**Flexibility:** React is just the view layer of the application, so it can be integrated with other libraries and frameworks. You can use React with Redux for state management, React Router for navigation, and other libraries to build a complete solution tailored to your needs.

4. ### React 19 Features
   <details>
   <summary>
   1. Concurrent Rendering
   </summary>
   Concurrent rendering is a set of new rendering behaviors in React that help apps stay responsive and gracefully adjust to the user’s device capabilities and network speed.

   **Automatic Batching:** Automatically batches updates inside promises, setTimeout, native event handlers, or any other event.

   **Transitions:** A new primitive for managing asynchronous state transitions, allowing for more fine-grained control over visual loading states.
   </details>

   2. **Suspense for Data Fetching**
Suspense, which was originally introduced in React 16.6 for code splitting, has been extended to support data fetching. This allows components to "wait" for something before they render.

3. React Server Components
Server Components allow developers to build apps that span the server and client, leveraging server-side rendering for better performance and user experience.

4. Automatic Batching
In React 18, React will batch updates that happen within the same event handler automatically, making the state updates more efficient.

5. Concurrent Features APIs
These are opt-in features for using concurrent rendering. Some new hooks and APIs have been introduced to help developers work with concurrent rendering:

useTransition: Helps in marking updates as non-urgent.
useDeferredValue: Helps in deferring the re-rendering of a non-urgent part of the UI.
startTransition: Similar to useTransition but for class components.
6. Streaming Server-Side Rendering (SSR)
React 18 introduces new APIs for server-side rendering that support streaming, allowing parts of the UI to be sent to the client as soon as they are ready, improving the time-to-first-byte (TTFB).

7. New Root API
React 18 introduces a new root API (createRoot) which is required to enable concurrent features.

8. New Hooks
Several new hooks have been introduced, primarily to support concurrent rendering:

useId: Helps to generate unique IDs for accessibility attributes.
useInsertionEffect: A hook to insert styles before mutations.
9. Improved SSR Hydration
Improved hydration process for server-rendered content, making it faster and more efficient.

10. ESM (ES Modules) Support
Enhanced support for ES Modules, aligning React with modern JavaScript module standards.


### What is Hooks


### Types of Hooks
state manaagement = useState,useReducer,useSyncExternalStore
Effect Hooks = useEffect, useLayoutEffect, useInsersionEffect
ref hooks = useRef, useImperativeHandle
Performance Hooks = useMemo, useCallback
Transition Hooks = useTransition, useDefernedValue
Context Hooks = useContext
Random Hooks = useDebugValue, useId
React 19 Hooks = useFormStatues, USeFormState, UseOptimistic, use


series

how react works
what is emmet
crossorigin in <script> tag
react and react-dom packages
render vs return 
async and defer
bundilers -vite, parcel, webpack
hot module replacement HMR
file watcher algorithm

transitive dependencies
browser list package-babel
pollyfill
tree shaking - removing unwanted code
react key reconcilliation
jsx - sanitization

components
functional and class based
component composition

//jsx mandodatory?

react.fragment


react fiber
why we not use index as key

react variable 

handle error in useEffect()

shimmer effect in ui

conditional rendering

{} in here JS expression will work not statement
statement -eg: let a = 10
expression - eg: console.log('hello'), ((a=10),console.log(a))

formik library

dynamic routing

object.values in javascript

tailwind and postcss
squrebracket notation (w-[200px])

prop drilling

pass data parent to child

lifting the state up (concept)

can we have nested context and context inside context

redux devtool extension 
jest
react testing library 
enzyme - old testing library 
why test cases
test driven development 

types of testing
e2e testing
unit testing
manual testing
automated testing 
integrated testing

babel
json vs js object
.toBe(5)

js dom

2:02
ffffff

react and react dom
event handlers
react props
controlled and uncontrolled elements
babel
class vs function
render
immutable
create-react-app
state - state rules

life cycle methods
1.constructor
2.render.
3.componentdidmount
4.componentdidupdate
5.componentwillunmound




bbbbbbbbbbbbbbbbbbbb
components
jsx
props
composition
rendering
virtual dom
diffing or diffs
reconciliation
event handling
states
controlled and uncontrolled components
types of hooks(state hooks, context hools, ref hooks, effect hooks , performance hooks)
purity
portals
suspense
error boundaries


## React Router

what is react router and why?
<BrowserRouter/>
<HashRouter/>
<Routes/>
<Route/>
<Link/>
<NavLink/>


url parameters vs search parameters
useParams, useSearchParams hook

relative path vs absolute path(it has '/')
default route <Route path="*" element={<notFound/>}>
useNavigate
useLocation()

nested route
descented routed
<outlet>
index route

dynamic routing
dynamic import
static bundling
code splitting
react.lazy
suspense
code bundling
protected routes
public routes
role based routes