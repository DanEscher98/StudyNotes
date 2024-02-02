# Memoization (in terms of set theory)

- A relation is just a subset of pairs
- These set relations forms a cartesian product
- So by definition, any subset of the cartesian product _is_ a relation
- Relations do not have directionality, but functions do
- A function can therefore be said to be a relation with directional
  constraints, namely those going from a domain (lhs) to a codomain (rhs) The
  following structure holds for invertible functions

```haskell
f :: a -> b
g :: b -> a
g after f = id
f after g = id
```

> This geometric understanding helps intuit a meaning for isomorphisms (and
> this is for isomorphisms in any given category.)
