---
created:
  - 2024-03-09 09:47
tags:
  - rust
  - programming
---
# Crates

https://crates.io/
The node package manager of the rust world

all project dependencies will be listed in Cargo.toml

Can use:
```
cargo add [CRATE]
```

or type into Cargo.toml and when building, it will download the latest version

Cargo.lock will have the packages necessary to run the crate.  It may not include what you installed, but may be used by the package in some form.
