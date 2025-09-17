# 📄 Installing Substrate Cargo Contract Node (v0.38.0)

This guide explains how to download, install, and run the **Substrate Cargo Contract Node** on Ubuntu (or WSL on Windows). This node is required for testing and deploying smart contracts built with [ink!](https://use.ink).

---

## 🛠 Prerequisites

* **Ubuntu** or **WSL2 on Windows** installed.
* `wget` and `tar` available (install them if missing):

  ```bash
  sudo apt update && sudo apt install wget tar -y
  ```

---

## 🚀 Installation Steps

### 1. Download the specific node version

Replace `<VERSION>` with the release version you want (e.g., `v0.38.0`):

```bash
wget https://github.com/paritytech/ink-node/releases/download/<VERSION>/ink-node-linux.tar.gz
```

---

### 2. Extract the tarball

Unpack the downloaded file:

```bash
tar -xzf ink-node-linux.tar.gz
```

---

### 3. Make the binary executable

```bash
chmod +x ink-node
```

---

### 4. (Optional) Move the binary to your PATH

This allows running `ink-node` from any directory:

```bash
sudo mv ink-node /usr/local/bin/
```

---

### 5. Verify the installation

Check the installed version:

```bash
ink-node --version
```

---

### 6. Run the node

Start the node in development mode:

```bash
ink-node --dev
```

Or simply:

```bash
./ink-node
```

*(Use `--help` to view available options)*

---

## 📚 Additional Tips

* **Persistent Background Service**: Consider using `screen`, `tmux`, or a [systemd service](https://www.freedesktop.org/software/systemd/man/systemd.service.html) to keep the node running in the background.
* **Upgrade**: To upgrade to a new version, repeat the steps with the updated `<VERSION>` and replace the existing binary.
* **Documentation**: For more details, check out [Parity’s ink! documentation](https://use.ink) or the [ink-node releases](https://github.com/paritytech/ink-node/releases).
