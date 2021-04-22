
### Install Rust (Ubuntu):
	$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
	
	$ rustup toolchain install nightly
	
### Install Cargo-fuzz :
	$ cargo install cargo-fuzz
	
### Examples :

##### Example 1:
```bash
	$ git clone https://github.com/servo/rust-url.git
	$ cd rust-url
	$ git checkout bfa167b4e0253642b6766a7aa74a99df60a94048
	$ cargo fuzz init
	$ cargo fuzz run
	$ cargo +nightly fuzz run fuzz_target_1
```

##### Example 2:
