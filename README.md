# React Trekkbag App

Made using:

- Javscript
- CSS
- React

# Notes:

1. Button - using `children` prop to pass button text

- E.g. `src/components/Button.jsx`

2. react-select package for dropdown select list using `<Select>` and sort function

- E.g. `src/components/ItemList.jsx`

3. useEffect and localStorage

- E.g. `src/context/ItemsContextProvider.jsx`

4. useMemo() is a hook to optimize performance by preventing expensive computations from being re-executed unnecessarily during component re-renders.

- E.g. Sorting array in `src/components/ItemList.jsx`

5. Context API as a cleaner way to do prop drilling

- E.g.`src/contexts/ItemsContextProvider.jsx` and `src/lib/hooks.js`

Issues with context api:

- Performance issues: needlessly re-renders all components that is using context even when the component doesn't use a specific function (e.g. Sidebar re-renders when items are added even when it does not need it)
- Lots of boilerplate: Verbose when there are many context providers,
- Difficult to get advanced features (e.g. middleware)

Solutions - Third Party State Management Libraries:

- Zustand
- Redux

6. Zustand

- E.g. `src/stores/itemsStore.js`
- We are able to select specifically what we want to use
- localStorage using persist()

# Source:

- ByteGrad Professionan React and Nextjs course
