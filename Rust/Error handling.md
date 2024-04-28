---
created:
  - 2024-03-09 09:53
tags:
  - rust
  - programming
---
# Error handling

.expect() : If it doesn't expect the outcome it will cause a panic, an unrecoverable error, and stop the program and print out our "error with parse" statement.  This makes it easier to read and write but also ignoring any possible errors other than something bad happened, try again...
```
guess.trim().parse().expect("Error with parse.");
```

if we check the definition of .expect():
```
 pub fn expect(self, msg: &str) -> T
    where
        E: fmt::Debug,
    {
        match self {
            Ok(t) => t,
            Err(e) => unwrap_failed(msg, &e),
        }
    }
```

We can take away the Ok() & Err() and customize error handling.
```
loop {
	...

	let guess: u32 = match guess.trim().parse() {
		Ok(num) => num,
		Err(e) => {
			println!("Error with parse, try again");
			continue;
		}
	}
}
```
So in this example, rather than having the program panic, it will continue with the next iteration in the loop until (string) guess is parsed as a u32 type.