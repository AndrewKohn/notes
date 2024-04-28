---
created:
  - 2024-03-09 09:54
tags:
  - rust
  - programming
---
# Macros

Macros are denoted with the "!" character.  Macros are naturally shortened and will expand upon compile time.  You may see it behave like a function, like in the println!() example, but it does a lot more complex stuff behind-the-scenes.

While you may not need to know what/how each macro performs, but you can look up definitions of macros to see what they actually do.

println!();
```
macro_rules! println {

() => {

$crate::print!("\n")

};

($($arg:tt)*) => {{

$crate::io::_print($crate::format_args_nl!($($arg)*));

}};

}
```
