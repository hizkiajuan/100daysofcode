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