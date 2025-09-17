# 📦 Installing Cargo-Contract v5.0.3 and Creating an ink! Smart Contract

This guide explains how to install **cargo-contract v5.0.3** and create, test, and build an ink! smart contract.

---

## 🛠 Prerequisites

* [Rust](https://www.rust-lang.org/tools/install) (v1.89 or compatible)
* `rustup` configured with WebAssembly target `wasm32-unknown-unknown`
* Ubuntu or WSL2 environment

---

## 🚀 Install Cargo-Contract v5.0.3

Use the following command to install or upgrade cargo-contract:

```bash
cargo install --force --locked cargo-contract --tag v5.0.3 --git https://github.com/use-ink/cargo-contract
```

> The `--force` flag reinstalls even if it’s already installed. The `--locked` flag ensures dependency lockfiles are respected.

---

## 📝 Create a New Smart Contract

Generate a new ink! project:

```bash
cargo contract new <project-name>
```

Replace `<project-name>` with your desired contract name.

---

## 📂 Navigate to the Project

Move into your project directory:

```bash
cd <project-name>
```

---

## ✅ Run Tests

Run the included unit tests:

```bash
cargo test
```

---

## 🏗 Build the Contract

Build the smart contract in debug mode:

```bash
cargo contract build
```

Or build in release mode for optimized output:

```bash
cargo contract build --release
```

---

## 📚 Additional Resources

* [Cargo-Contract v5.0.3 Release Notes](https://github.com/use-ink/cargo-contract/releases/tag/v5.0.3)
* [ink! Documentation](https://use.ink)
