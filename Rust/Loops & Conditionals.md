---
created:
  - 2024-03-09 09:50
tags:
  - rust
  - programming
---
# Loops & Conditionals

#### if / else if expressions
```
if guess == correct {
	println!("Correct!");
} else {
	println!("INCORRECT!");
}
```

Usually if & else if are conditional statements.  In rust, it's treated as conditional expressions.  Reason for this is that you can return a value as part of a binding or larger expression.

```
let guess: u32 = 44;
let correct: u32 = 44;

......

let message = if correct < guess {
	"TOO HIGH";
} else if correct > guess {
	"TOO LOW";
} else {
	"AYYYYY LETS GO";
}

println!("{message}");

// output: "AYYYYY LETS GO"

```

#### Loops
loop will keep looping and it's our responsibility to handle how we get out of that mess.
```
loop {
...
break;
}
```

break : will break out of the loop entirely
continue : will stop the current iteration and move onto the next iteration, essentially will not run any code past that statement for that iteration.

While loop:
```
let mut num = 120;
let mut count = 0

while count < num {
...
count += 1;
}

println("count: {count}");

// output: "count: 119"
```

for...in loop
```
let mut items = Vec::new();

...

for item in items {
	println!("{item}");
}
```
