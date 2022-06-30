# react-tmg
React fundamentals apps with inline scripts based on Tyler McGinnis' walkthroughs, but using hooks instead of classes and React 18. Heavily annotated.

## Important disclaimer
I'm not using branches the way they're meant to be used. You can check out main branch for day 1 and the next branches for day 2, 3, etc.

## Day 2
Have only been using `return` for elements and not at all inside 'handler' functions.
So much better with hooks because you don't have to deal with the need to .bind anything (classes usage).

## Day 3 (day-3-loading)
I'm not successfully fooling Suspense or able to use React.lazy to simulate in current setup. Currently the "loader" is therefore not a good representation of actual approach.

## Day 3 hw (day-3-hw)

Why cannot use arrow function inside the return of a component (RepoChoice)? 🤔
  - "solution": with `{choices}.map(...)` ".map is not a function" - not recognizing the array variable. Use simply `choices.map(...)`
Taking useCallback out for a spin, thanks to useEffect: [here](https://reactjs.org/docs/hooks-reference.html#usecallback)
  - useCallback: otherwise a new instance of the function keeps getting created, and not equal. But [how](https://infinitypaul.medium.com/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3).
  - useRef? "useRef doesn’t notify you when its content changes. Mutating the .current property doesn’t cause a re-render." Maybe a good thing if I don't want useEffect to run again and want to rerender just with set_State_-callbacks? Warning [here](https://medium.com/@teh_builder/ref-objects-inside-useeffect-hooks-eb7c15198780)
