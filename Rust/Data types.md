---
created:
  - 2024-03-09 09:52
tags:
  - rust
---
# Data types

"&" = referencing
"mut" = mutable
e.g. &str

### String
static:
```
let name = "Andy";  // String literal
```

dynamic:
```
let name = String::new();
```

`String` is an owned grownable UTF-8 encoded string. The term "owned" means that a variable `s` of type `String` has ownership over the content of the string. When `s` goes out of scope the owned string is dropped.
```
...  
{ // New scope  
    let s: String = String::from("My string"); // "My string" is owned by s  
    ...  
} // End of scope, `s` and the owned string "My string" are dropped  
...
```
Internally in the standard library, as defined as:

```
pub struct String {  
    vec: Vec<u8>,  
}
```

Yes, exactly, a `String` is just a vector of bytes (`u8`). However, the standard library implementation of `String`ensures that the array of bytes pointed by `vec` actually contains only valid UTF-8 bytes.

### &str
str is a "string slice", a sequence of bytes in memory that is known to be valid UTF-8 text. It's a primitive type in Rust and most of the time is used in its borrowed form &str.

The reason for this is that str is not a Sized type, meaning that its size is not known statically (at compile time) and the Rust compiler must know the size of all the local variables in order to guarantee the security features provided by the Rust language.

`str` does not implement `Sized` trait and therefore its size is not known statically at compile time.

