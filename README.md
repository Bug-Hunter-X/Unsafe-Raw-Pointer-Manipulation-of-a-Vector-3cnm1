# Unsafe Raw Pointer Manipulation of a Vector in Rust

This repository demonstrates a common error when using raw pointers in Rust to interact with vectors. Modifying a vector's elements through a raw pointer after the vector's ownership has changed can lead to undefined behavior and memory corruption.

The `bug.rs` file shows the erroneous code, while `bugSolution.rs` provides a safe alternative using vector indexing.  The core issue is accessing memory after the vector's allocation may have been released.