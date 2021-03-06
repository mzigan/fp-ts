---
title: Random.ts
nav_order: 63
parent: Modules
---

# Random overview

Added in v2.0.0

---

<h2 class="text-delta">Table of contents</h2>

- [randomBool (constant)](#randombool-constant)
- [random (function)](#random-function)
- [randomInt (function)](#randomint-function)
- [randomRange (function)](#randomrange-function)

---

# randomBool (constant)

Returns a random boolean value with an equal chance of being `true` or `false`

**Signature**

```ts
export const randomBool: IO<boolean> = ...
```

Added in v2.0.0

# random (function)

Returns a random number between 0 (inclusive) and 1 (exclusive). This is a direct wrapper around JavaScript's
`Math.random()`.

**Signature**

```ts
export const random: IO<number> = () => ...
```

Added in v2.0.0

# randomInt (function)

Takes a range specified by `low` (the first argument) and `high` (the second), and returns a random integer uniformly
distributed in the closed interval `[low, high]`. It is unspecified what happens if `low > high`, or if either of
`low` or `high` is not an integer.

**Signature**

```ts
export function randomInt(low: number, high: number): IO<number> { ... }
```

Added in v2.0.0

# randomRange (function)

Returns a random number between a minimum value (inclusive) and a maximum value (exclusive). It is unspecified what
happens if `maximum < minimum`.

**Signature**

```ts
export function randomRange(min: number, max: number): IO<number> { ... }
```

Added in v2.0.0
