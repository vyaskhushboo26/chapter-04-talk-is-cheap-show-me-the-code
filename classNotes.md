1. Recap on Chapter-03 - functional component, react elements

2. Creating food ordering app - Food Villa in this session

3. Writing comments in jsx

4. We don't need ES6, jsx, typescript to work in react

5. Good notes app - for UX planning

-> Create low level design -> Create app layout

- header
    - logo (Title)
    - nav items (right side)
    - cart

- body
    - search bar
    - restaurantCard
    - restaurantList
    - image
    - Name
    - Rating
    - Cuisine
- footer

-> Create HeaderComponent -> Add TitleComponent -> it has logo img and a tag for the image. -> div nav-items (ul and li )

-> Create Body and Footer Component

-> Create AppLayout -> put header, body and footer within <></>

JSX has only one parent ->use React.Fragment -> its like empty tag -> <> </>

but if you want to give attrbutes, style -> div tag

style = { border : red 1px soild} ; -> not possible -> wrap inside () inside jsx

Config - driven UI : Different UI layout for different users - Backend driven config

Optional chaining ?

Props (Properties) -> attributes passed through component tag -> similar to arguments passed in function in js -> received as parameters in the function (component in react)

: const Component = (props)=>{()} :: func(arguments) : const func = (parameters) => {}

Virtual DOM -> representation/copy of DOM with us

Purpose : React Reconciliation -> React uses diff Algorithm to find out the difference between one tree (actually dom) from another which determines what needs to be updated and only re-renders the diff

re-render everything if key is not mentioned

react fiber -> it comes in react 16. its a new reconciliation engine and this engine is responsible for DIFF.

never use index as key

no key(not acceptable) < index key(only use if dont have anything) < unique key(best practices)