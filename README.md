# Vebex

Vebex is a Rust library that provides procedural macros for creating regular expressions in a verbose and readable way.

## Features

- Create regular expressions using a more readable syntax.
- Compile-time validation of regular expressions.
- Integration with Rust's standard `regex` crate.

## Installation

Add the following to your `Cargo.toml`:

```toml
[dependencies]
vebex = "0.1.0"
```

## Usage

```rust
use vebex::regex;

let re = regex! {
    start_of_line
    "hello"
    one_or_more_whitespace
    "world"
    end_of_line
};

assert!(re.is_match("hello world"));
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.