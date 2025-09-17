## docs

### Installing Substrate Cargo Contract Node (v.38.0)

1. Open Ubuntu WSL to download the specific node version
     ```bash
     wget https://github.com/paritytech/ink-node/releases/download/<VERSION>/ink-node-linux.tar.gz
     ```

2.  Extract the tarball file
     ```bash
     tar -xzf ink-node-linux.tar.gz
     ```

3.  Make the node executable
     ```bash
     chmod +x ink-node
     ```

3.  Run the node
     ```bash
     ./ink-node
     ```
