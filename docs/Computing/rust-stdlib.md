# Rust Standard Library

## Core Primitive types
- `bool`: The boolean type.
- `pointer`: Raw, unsafe pointers, *const T, and *mut T.
- `reference`: References, &T and &mut T.
- `fn`: Function pointers, like `fn(usize) -> bool`.
- `never`: The `!` type, also called “never”.
- `unit`: The `()` type, also called “unit”.
- `tuple`: A finite heterogeneous sequence, `(T, U, ..)`.
- `core::array`: A fixed-size array, denoted `[T; N]`, for the element type,
  `T`, and the non-negative compile-time constant size, N.
- `core::slice`: A dynamically-sized view into a contiguous sequence, `[T]`.
    Contiguous here means that elements are laid out so that every element is
    the same distance from its neighbors.
- `core::char`: A character type.
- `core::str`: String slices.
- `core::f{32, 64}`: A floating point type (specifically IEEE 754-2008).
- `core::i{8, 16, 32, 64, 128, size}`: The signed integer type.
- `core::u{8, 16, 32, 64, 128}`: The unsigned integer type
- `core::usize`: The pointer-sized unsigned integer type.

## Common types and Collections
- `primitive`: This module reexports the primitive types to allow usage that is
  not possibly shadowed by other declared types.
- `core::ascii`: Operations on `ASCII` strings and characters.
- `core::hash`: Generic hashing support.
- `core::iter`: Composable external iteration.
- `core::num`: Additional functionality for numerics.
- `core::cmp`: Utilities for comparing and ordering values.
- `core::ops`: Overloadable operators.
- `core::option`: Optional values.
- `core::result`: Error handling with the Result type.
- `alloc::string`: A `UTF-8`–encoded, growable string.
- `alloc::vec`: A contiguous growable array type with heap-allocated contents,
  written `Vec<T>`.
- `alloc::collections`: Collection types.
- `alloc::fmt`: Utilities for formatting and printing `Strings`.

## Smart Pointers, Containers and Memory
- `core::alloc`: Memory allocation APIs.
- `core::any`: Utilities for dynamic typing or type reflection.
- `core::borrow`: A module for working with borrowed data.
- `core::clone`: The `Clone` trait for types that cannot be "implicitly
    copied".
- `core::cell`: Shareable mutable containers.
- `core::mem`: Basic functions for dealing with memory.
- `core::pin`: Types that pin data to its location in memory.
- `core::ptr`: Manually manage memory through raw pointers.
- `core::sync`: Useful synchronization primitives.
- `alloc::boxed`: The `Box<T>` type for heap allocation.
- `alloc::rc`: Single-threaded reference-counting pointers. `Rc` stands for
  ‘Reference Counted’.

## Synchronous, Asynchronous and Concurrency
- `core::future`: Asynchronous basic functionality.
- `core::task`: Types and Traits for working with asynchronous tasks.
- `std::process`: A module for working with processes.
- `std::thread`: Native threads.

## Types and Traits
- `core::convert`: Traits for conversions between types.
- `core::default`: The `Default` trait for types with a default value.
- `core::marker`: Primitive traits and types representing basic properties of
  types.

## `IO`, `OS` and Network features
- `core::arch`: `SIMD` and vendor intrinsics module.
- `core::ffi`: Utilities related to `FFI` bindings.
- `core::hint`: Hints to compiler that affects how code should be emitted or
    optimized. Hints may be compile time or runtime.
- `core::panic`: Panic support in the standard library.
- `core::time`: Temporal quantification.
- `std::backtrace`: Support for capturing a stack backtrace of an OS thread
- `std::env`: Inspection and manipulation of the process’s environment.
- `std::error`: Interfaces for working with `Errors`.
- `std::fs`: Filesystem manipulation operations.
- `std::io`: Traits, helpers, and type definitions for core `I/O`
    functionality.
- `std::net`: Networking primitives for `TCP/UDP` communication.
- `std::os`: OS-specific functionality.
- `std::path`: Cross-platform path manipulation.
