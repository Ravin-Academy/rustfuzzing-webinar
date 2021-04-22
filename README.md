
### Install Rust (Ubuntu):
```bash
	$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
	
	$ rustup toolchain install nightly
```
	
### Install Cargo-fuzz :
```bash
	$ cargo install cargo-fuzz
```

### Examples:

##### Example 1:
```bash
	$ git clone https://github.com/servo/rust-url.git
	$ cd rust-url
	$ cargo fuzz init
	$ cargo +nightly fuzz run fuzz_target_1
```

##### Example 2:
```bash
	$ git clone https://github.com/alexcrichton/rustc-demangle.git
	$ cd rustc-demangle
	$ cargo fuzz init
	$ cargo +nightly fuzz run fuzz_target_1
	
```

##### Example 3:
```bash
	$ git clone https://github.com/serde-rs/json
	$ cd json
	$ cargo +nightly fuzz run from_slice
```

##### Example 4:
```bash
	$ git clone https://github.com/zeta12ti/parse_duration.git # https://rustsec.org/advisories/RUSTSEC-2021-0041.html
	$ cd parse_duration
	$ cargo fuzz init
	$ cargo +nightly fuzz run fuzz_target_1
```


