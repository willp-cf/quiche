# How to build quiche for iOS

To get libquiche in iOS environment, you need to have

- Install xcode command line tools: you can install it with Xcode or the following command:

```
xcode-select --install
```

- Install cross compiling toolchains for rust:

```
rustup target add aarch64-apple-ios armv7-apple-ios armv7s-apple-ios x86_64-apple-ios i386-apple-ios
```

- Install `cargo-lipo`.

```
cargo install cargo-lipo
```

To build iOS binary, please run the following command:

```
cargo lipo
```

or

```
cargo lipo --release
```
