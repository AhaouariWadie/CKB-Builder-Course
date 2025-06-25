# Weekly Progress Report  
**Week:** 19 June 2025 – 25 June 2025  
**Author:** Ahaouariwadie (GitHub username)

---

## Summary of Activities

### 19 June 2025
- Began troubleshooting Ubuntu system access issues:  
  - Investigated root access and sudo command problems  
  - Encountered and diagnosed `dpkg` lock error and `sudo` missing  
  - Attempted password recovery and root access enabling  
- Commands used:  
  ```bash
  su
  sudo apt install sudo
  sudo apt install curl
  ```

### 20 June 2025
- Installed essential tools on Ubuntu VM to support Nervos course setup:  
  - Installed Git from source tarball after missing prebuilt binaries  
  - Verified Git installation and configuration  
- Commands used:  
  ```bash
  tar -xzf git-2.50.0.tar.gz
  ./configure
  make
  sudo make install
  git --version
  ```

### 21 June 2025
- Installed and configured Node.js V18 manually on Ubuntu VM:  
  - Downloaded and extracted Node.js tarball  
  - Moved Node.js files to `/usr/local` directory  
  - Updated PATH environment variable for easy access  
- Commands used:  
  ```bash
  tar -xJf node-v18.20.8-linux-x64.tar.xz
  sudo mv node-v18.20.8-linux-x64 /usr/local/node-v18.20.8
  export PATH=/usr/local/node-v18.20.8/bin:$PATH
  node -v
  ```

### 22 June 2025
- Started syncing CKB node and explored node sync status commands:  
  - Monitored sync progress via RPC calls  
  - Observed increasing best known block number with `ibd` flag true  
- Commands used:  
  ```bash
  ./ckb-cli rpc sync_state
  ./ckb-cli rpc get_tip_header
  ```

### 23 June 2025
- Worked on making the CKB node discoverable on the Node Probe map:  
  - Edited `ckb.toml` to set proper `node_announce` and `public_endpoint` configuration  
  - Restarted the node and checked logs for discoverability  
- Commands used:  
  ```bash
  nano ~/.ckb/ckb.toml
  systemctl restart ckb
  journalctl -u ckb -f
  ```

### 24 June 2025
- Debugged Ubuntu file permission and root access issues during CKB setup:  
  - Used `find` command to locate Rust installation  
  - Managed permission errors related to package installs and file locks  
- Commands used:  
  ```bash
  find ~/local/rust-1*
  sudo chown -R ubuntu:ubuntu ~/.cargo
  sudo rm /var/lib/dpkg/lock-frontend
  ```

### 25 June 2025
- Followed Nervos documentation to run a Devnet node:  
  - Cloned devnet configuration files and genesis block data  
  - Started the node in devnet mode using updated configuration  
  - Verified node synchronization on devnet  
- Main steps (from https://docs.nervos.org/docs/node/run-devnet-node):  
  1. Download and extract the latest CKB binary  
  2. Create a new config folder and copy devnet config files  
  3. Modify `ckb.toml` to use devnet genesis hash and chainspec  
  4. Start the CKB node with `--chain dev` flag  
  5. Check node logs for sync status and peers connection  
- Commands used:  
  ```bash
  wget https://github.com/nervosnetwork/ckb/releases/download/v0.202.0/ckb_v0.202.0_x86_64-unknown-linux-gnu.tar.gz
  tar -xzf ckb_v0.202.0_x86_64-unknown-linux-gnu.tar.gz
  mkdir ~/.ckb_dev
  cp -r config/devnet/* ~/.ckb_dev/
  ./ckb --chain dev --ba --indexer
  tail -f ~/.ckb_dev/logs/ckb.log
  ```

---

## Challenges & Notes
- Initial Ubuntu environment setup was hindered by missing sudo and permission issues, delaying package installations.
- Manual installation of Git and Node.js ensured environment compatibility but added complexity.
- Monitoring and syncing CKB nodes required understanding of RPC commands and log interpretation.
- Configuring CKB node discoverability involved detailed edits to the `ckb.toml` configuration file.
- Devnet node setup finalized with successful startup and synchronization confirmation as per Nervos docs.

---

## Goals for Next Week
- Complete smart contract labs on the CKB devnet  
- Automate node setup scripts for faster deployment  
- Begin learning Rust basics relevant to CKB development  
- Explore dApp development with TypeScript and CKB SDK

---
