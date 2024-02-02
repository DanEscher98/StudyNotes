# Rust Keywords

## Conditional and Loop Structures
- **break** exit a loop immediately
- **continue** continue to the next loop iteration
- **for** loop over items from an iterator
- **in** part of for loop syntax
- **loop** loop unconditionally
- **while** loop conditionally based on the result of an expression
- **if** branch based on the result of a conditional expression
- **else** fallback for if and if let control flow constructs
- **false** Boolean false literal
- **true** Boolean true literal

## Functions and Variables
- **fn** define a function or the function pointer type
- **return** return from function
- **const** define constant items or constant raw pointers
- **let** bind a variable
- **move** make a closure take ownership of all its captures
- **mut** denote mutability in references, raw pointers, or
    pattern bindings
- **ref** bind by reference
- **static** global variable or lifetime lasting the entire program
    execution

## Data Structures, Functions and Variables
- **as** perform primitive casting, disambiguate the specific
    trait containing an item
- **enum** define an enumeration
- **impl** implement inherent or trait functionality
- **for** implement a trait, or specify a higher-ranked lifetime
- **match** match a value to patterns
- **Self** a type alias for the type implementing a trait
- **self** method subject
- **struct** define a structure
- **trait** define a trait
- **type** define a type alias or associated type
- **where** denote clauses that constrain a type

## Modules and Others
- **as** rename items in use and extern crate statements
- **crate** link an external crate or a macro variable
    representing the crate in which the macro is defined
- **self**, current module
- **extern** link an external crate, function, or variable
- **mod** define a module
- **pub** denote public visibility in struct fields, impl
    blocks, or modules
- **super** parent module of the current module
- **use** import symbols into scope

## Dark Arts
- **unsafe** denote unsafe code, functions, traits, or implementations
- **async** return a `Future` instead of blocking the current thread
- **await** suspend execution until the result of a `Future` is ready
- **macro_rules!** define declarative macros

## Syntax miscellanious
- `&`: reference operator
- `*`: dereference operator
- `|e| { ... }`: lambda syntax
- `_`: wildcard
- `'_`: lifetime
- `!`: never
- `()`: unit type
- `(T, U, ..)`: tuple
- `[T; N]`: fixed-size array
- `&[T]`: slice
- `foo::<T>()`: turbofish
- `?`: propagate operator

## REFERENCES
- [Operator expressions](https://doc.rust-lang.org/reference/expressions/operator-expr.html)
