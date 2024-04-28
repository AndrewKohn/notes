---
created:
  - 2024-03-09 09:55
tags:
  - rust
  - programming
---
# Vector

Vectors are a dynamic collection that allows us to store multiple elements, and we can add elements onto it.

```
let num_guesses: u8 = how_many_guesses.trim().parse().expect("Error reading input");
let mut answers = Vec::new();

for i in 0..num_guesses {
	answers.push(rand::thread_rng().gen_range(1..=10));
}

println!("{answers:?}");

// input: How many guesses: 5
// output: [9, 3, 5, 1, 5]

```