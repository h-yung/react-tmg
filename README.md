# React fundamentals via TMG
React fundamentals apps with inline scripts based on Tyler McGinnis' walkthroughs, but using hooks instead of classes and React 18. Heavily annotated.

## Important disclaimer
I'm not using branches the way they're meant to be used. You can check out main branch for day 1 and the next branches for day 2, 3, etc.

## Day 2
**Below: A list similar to to-do list, minus edit capabilities**<br>
<img src="https://raw.githubusercontent.com/h-yung/react-tmg/main/day-2-hw.png?token=GHSAT0AAAAAABVMLGSR4UAD7EWCAXBRQRVQYV6DMKA" alt="day 2 screen" width="200"/> 

Have only been using `return` for elements and not at all inside 'handler' functions.
So much better with hooks because you don't have to deal with the need to .bind anything (classes usage).

## Day 3 (day-3-loading)

**Below: Updates with top repositories for the specified language. Default is "all."**<br>
<img src="https://raw.githubusercontent.com/h-yung/react-tmg/main/day-3-hw.png?token=GHSAT0AAAAAABVMLGSQVMULAJNTJSF64JDOYV6DIWQ" alt="day 2 screen" width="500"/>

I'm not successfully fooling Suspense or using React.lazy to simulate in current setup for the "loading" interim component.
**Incomplete:** Loader interim component.

## Day 3 hw (day-3-hw)

Some errors while attempting to use the arrow function inside the return of a component (RepoChoice). 🤔
  - "solution": with `{choices}.map(...)` ".map is not a function" - not recognizing the array variable. Use simply `choices.map(...)`
  Taking useCallback out for a spin, thanks to useEffect: [here](https://reactjs.org/docs/hooks-reference.html#usecallback) to avoid a new instance of the function getting created each time. [Reference used](https://infinitypaul.medium.com/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3).
  - useRef? "useRef doesn’t notify you when its content changes. Mutating the .current property doesn’t cause a re-render." I did not use it here. Warning [here](https://medium.com/@teh_builder/ref-objects-inside-useeffect-hooks-eb7c15198780)

