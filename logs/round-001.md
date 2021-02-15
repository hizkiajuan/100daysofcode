# Round 001

## Day 001 - 20210201
### Progress
- start with FCC's curriculum : continue JavaScript Algorithms and Data Structures Certification
- got 3 questions about recursion : loop to recursion, countdown array, range of numbers
### Thoughts
- glad and excited to get up and running on this challenge
- it is time to achieve the other certifications
- need to grasp more understanding about how recursion works
### Link
- got one achievement before in [Responsive Web Design](https://www.freecodecamp.org/certification/hizkiajuan/responsive-web-design) certification

---

## Day 002 - 20210202
### Progress
- finish FCC's ES6 curriculum : module import/export, promise
- dig deeper about Promise on [javascript.info](https://javascript.info/async)
- javascript.info (2/8 topics) : learn about "callback-based" async, Promise intro
### Thoughts
- syntax `import { something } from 'somewhere.js'` similar to object destructuring `const { something } = somewhere.js`
- a `new Promise()` syntax indicates a "constructor function"
- Promise-thing : resolve, reject, then, catch, finally
- `finally` will pass through any result (or error) to its next handler
- only the first resolve/reject call that is taken into account

---

## Day 003 - 20210203
### Progress
- continue javascript.info (5/8 topics) about Promise
- topics : Promise chaining, error-handling, API
### Thoughts
- a handler in Promise (then/catch/finally) may return not exactly a Promise, but a so-called "thenable" object (an arbitrary object that has a method `.then`)
- "thenable" object will be treated the same way as Promise
- there is an "invisible" `try...catch` block in a Promise
- `catch` handles `reject` as well as an Error `throw` (in a synchronous way)
- `Promise.all` : got a `reject` in the middle, it will ignore the rest Promise(s)
- `Promise.allSettled` : fulfill all Promise, return both sucess and error
- `Promise.race` : return the only first _settled_ Promise (success or error)
- `Promise.any` : return the only first _fulfilled_ Promise (success only) - if all rejected, return `AggregateError`

---

## Day 004 - 20210204
### Progress
- will revisit javascript.info topic 6-8 about Promise later.. together with async/await (I _promise_!)
- continue FCC about Regex : literal match, any match, (negated) character class/set, one/zero or more match, OR,  flags, lazy match, caret/sign character, (opposite) alphanumeric (_shorthand_ of character class), (non) digit match
- stuck on [Restrict Possible Usernames](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/regular-expressions/restrict-possible-usernames), but will try again tomorrow
### Thoughts
- [regex by default is _greedy_](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/regular-expressions/find-characters-with-lazy-matching) (match the **longest** possible part)
- add `?` to make it _lazy_ (match the **shortest** possible part)
- alphanumeric match using `\w` also includes `_` character

---

## Day 005 - 20210205
### Progress
- continue FCC's regex : (non) whitespace, quantity specifier (lower/upper number), check for all or none, [lookahead pattern](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/regular-expressions/positive-and-negative-lookahead), character grouping, capture group, search+replace by capture groups
### Thoughts
- just discover there is a `"string".repeat(n)`
- hard to understand : lookahead `(?=...)` and capture group `\1`
- _capture group_ is kinda copy+paste, no?

---

## Day 006 - 20210206
### Progress
- still in FCC, but now : Debugging
- topics covered : `console.log`, `typeof`
- revisit loose/abstract vs strict/identity equality
### Thoughts
- 3 types of errors: syntax, runtime and semantic/logical error
- OBOE : off-by-one error (e.g. access wrong index)

---

## Day 007 - 20210207
### Progress
- off I go to FCC's OOP
- topics covered : constructor, `new`, `instanceof`, `own` and `prototype` property, special `constructor` property, `isPrototypeOf`, `prototype` chain, `Object.create()`, _override_ inherited methods, "mixins" concept, closure, IIFE
### Thoughts
- keyword `this` in an `object` refer to _that_ object (firstly)
- `constructor` has first letter uppercased, but `function` all lowercase
- just figured out the difference of `own` and `prototype` properties
- manually set an object `prototype` prop will **erase** its `constructor` prop, [add one each time define them!](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/remember-to-set-the-constructor-property-when-changing-the-prototype)
- "all" JS objects have a `prototype`, which the `prototype` itself is an `object` (`Object` is _supertype_ of all JS objects -> [prototypal inheritance](https://www.freecodecamp.org/news/all-you-need-to-know-to-understand-javascripts-prototype-a2bff2d28f03/) (😮can't believe I wrote this - now it's just make sense)
- use "mixins" to combine/"inherit" properties from different type of object (e.g. `fly` prop that is being used by bird & plane)
- closure is simply a "context scope" that defines accessibility of props
- IIFE is usually used [to create a module](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-an-iife-to-create-a-module) -> can be achieved by just creating an object, IIFE just return the value right away

---

## Day 008 - 20210208
### Progress
- move on to Functional Programming from #freeCodeCamp
- topic covered : callbacks, first class function, higher order function, lambda, imperative vs declarative, splice vs slice, mutation, side-effect, pure function
### Thoughts
- in JS, all functions are first-class function
- functional prog principle : declare your dependencies explicitly

---

## Day 009 - 20210209
### Progress
- Functional Programming cont.
- topic covered : map + filter (and how to build them manually), slice (return new arr), splice (mutate original arr), concat, reduce
### Thoughts
- on FCC : once solve the problem, go to Hint page to see the other POV on how to solve it
- it's not that hard to implement our own map/filter function
- `splice` is all about "remove and join" : remove items on given index range, then join the left & right side of arr items

---

## Day 010 - 20210210
### Progress
- Function Programming cont. (last)
- topic covered : sort, sort without mutating (use concat), split, join, every, some, currying, partial applicaiton with `bind`
### Thoughts
- the most eplxainable definition of currying (from FCC) : convert N-arity function into N-function of 1 arity

---

## Day 011 - 20210211
### Progress
- continue FCC curriculum : Basic Data Structures
- topic covered (1) array : push + unshift, pop + shift, splice, slice, spread operator, indexOf
- topic covered (2) object : accessing (nested) object, bracket notation, delete, hasOwnProperty, for...in, Object.keys()
### Thoughts
- just realized that push/unshift can receives multiple arguments
- \>= 3rd param of `splice` means insert to arr at front

---

## Day 012 - 20210212
### Progress
- into the Algorithms (Basic)
- topic covered : reverse string (split/reverse/join), factorial (basic for loop), longest/largest word/number in string/array (reduce), `.endsWith()` alternative with slice, `.repeat()` alternative with `while` loop
### Thoughts
- watch out if returning `arr.push()` in reduce : it returns [new length of array](https://stackoverflow.com/a/41890580/6147996)
- many string problem can be solved with convert it first to array (may not efficient tho)

---

## Day 013 - 20210213
### Progress
- Algorithms (Basic) cont.
- topic covered : array find using callback function, check if primitive boolean using typeof, replace with charAt, slice with concat, filter with boolean casting
### Thoughts
- Scripting section on FCC has (mostly) no clue/hint on the question so they let me think it on my own -> that's why it trains our logical thinking about algo + DS
- [Where do I belong](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-algorithm-scripting/where-do-i-belong) made my day!
- array operation can be applied on string (indexOf, includes, etc)

---

## Day 014 - 20210214
### Progress
- comes into Intermediate Algorithms
- topic covered : sum all numbers in range (really [worth-to-read Hint](https://forum.freecodecamp.org/t/freecodecamp-challenge-guide-sum-all-numbers-in-a-range/16083)), diff two arrays (again, the Hint gave me another perspective)
### Thoughts
- it is worth to look at the Hint section once we solve the problem : learn from various POV

---

## Day 015 - 20210215
### Progress
- some urgent matters today, so I can't continue the FCC progress
- but, I made progress on hizkiajuan.com v3.0 (hopefully it is *counted* here)
### Thoughts
- to start may difficult, but to continue (consistent) is more difficult
- anyway, besides #100DaysOfCode I also commit on finishing the hizkiajuan.com v3.0 :) #KeepItUp!