---
created:
  - 2024-03-09 09:54
tags:
  - rust
---
# Variables

```
let name = "Andy";
println!("Hello {name}!");

// output = "Hello Andy!"
```

The above code is not an assignment, but we are kind of assigning a value to our variable.  This is called a binding in rust.  This establishes who is responsible for that memory and where that memory is stored.

Variables are immutable.  We are unable to give the name variable a new value.

```
let mut name = "Andy";
name = "Bubba";
println!("Hello {name}!");

// output = "Hello Bubba!"
```

You can label variables as mutable with the "mut" and this will allow us to mutate the value through out the code.

There are other ways to insert variables:
```
let name = "Andy";
let country = "USA";
println!("Hello {name} from {country}!");  // Inside brackets

// output = "Hello Andy from USA!"
```

```
let name = "Andy";
let country = "USA";
println!("Hello {} from {}!", name, country);  // Outside of brackets

// output = "Hello Andy from USA!"
```

You can insert a variable inside the brackets if you're going to use just that variable, but if you're performing any functions, operations, calculations, etc..., then you would need to put your variable outside.
```
let name = "Andy";
let country = "USA";
println!("Hello {name} from {}!", country.to_lowercase());  // both

// output = "Hello Andy from usa!"
```

Say you want to print out your data in the terminal but doing this won't work:
```
let data = [1, 2, 3, 4, 5];
println!("{data}");
```

You'll have an error with std::Display and it won't run properly.

You can instead do this for debugging:
```
let data = [1, 2, 3, 4, 5];
println!("{data:?}");
// or
// println!("{:?}", data);

// output: [1, 2, 3, 4, 5]
```

You won't have much control with how it's displayed, but it's nice to use to display data in terminal quickly.

---

Rust is statically typed, but you can have a two variables with different types, yet same name in the same scope.  Rust will check for the correct type depending on implementation.
```
let guess: String = "32";
let correct: u32 = 44;
let guess: u32 = guess.trim().parse().expect("Error with parse");

if guess == correct {  // u32 guess and u32 correct comparison
...
} else {
...
}
```