# Rust Raw Pointer and Vector Reallocation Bug

This repository demonstrates a common error in Rust: dereferencing a raw pointer after a vector's capacity has changed.  The code attempts to read from a raw pointer to a vector after the vector has been reallocated due to a `push` operation. This leads to undefined behavior.  The solution shows how to avoid this issue by using safe Rust techniques.