
1. How to pass data from a child to parent?
	- The child component can use a function in the props/state which the parent can then bind to.
2. How to render an element outside of the component scope/tree?
	- Use React createPortal and specify the HTML element you where you want it to render
3. How to implement code splitting (lazy loading) in your React app and why?
	-  Utilize Reacts lazy, which uses JavaScript promises to lazy load components.
	- Use the callback in lazy to specify the path of the component(s) you want to lazily load.
	- You then call the component in the HMTL inside of `<Suspense> ` tags.
	- You can also specify fallback HTML to take it's place while the component is being loaded.
	- The lazy function will separate the component into a separate directory when the application compiles using JSX which is why it is called "code splitting"
1. What is the best way to add a global store to your React app or project?
	- Depending on what your app needs.... blah blah blah
	- Use Redux Toolkit
	- Create a store which contains "slices" that have reducers.
	- Reducers are the effect
	- Slices are the containers for functional logic for reducers
	- Stores store slices to be used
	- Import a Provider that will allow you to pass the store and specify the slices per component or view
1. Give me an example of a basic React SSR implementation?
	- SSR is most popularly used by Next.js
	- Server Side Rendering (SSR)



<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/3BN-YHcJfOY?si=LtqrG0QWDmZjLu0-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 4px;"></iframe>
