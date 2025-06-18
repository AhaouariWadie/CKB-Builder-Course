# Weekly Progress Report  
**Week:** 11 June 2025 – 18 June 2025  
**Author:** Ahaouariwadie (GitHub username)

---

## Summary of Activities

### 11 June 2025
- Completed the course: [Basic Theory](https://academy.ckb.dev/courses/basic-theory)

### 12 June 2025
- Completed the course: [Basic Operation](https://academy.ckb.dev/courses/basic-operation)

### 13 June 2025
- Started the [Nervos Developer Training Course](https://nervos.gitbook.io/developer-training-course)
- Learned blockchain basics from [dcxlearn.com](https://dcxlearn.com/blockchain/)
- Watched the following YouTube videos:  
  - [Blockchain Expert Explains One Concept in 5 Levels of Difficulty | WIRED](https://www.youtube.com/watch?v=l5J9fqXdkrI)  
  - [How Bitcoin Works Under the Hood](https://www.youtube.com/watch?v=_160oMzblY8&t=81s)  
  - [Bitcoin Mining in 5 Minutes](https://www.youtube.com/watch?v=6Fa04MnURhw&t=1328s)  
  - [Blockchain Technology Explained](https://www.youtube.com/watch?v=bBC-nXj3Ng4)

### 14 June 2025
- Began learning basics of programming languages via the Nervos course links:  
  - [JavaScript](https://javascript.info/)  
  - [TypeScript](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)

### 15 June 2025
- Installed and configured required software per Nervos Developer Training Course:  
  - Installed Rust toolchain and environment (did not study Rust basics yet)  
  - Installed Node.js V18 using NVM  
  - Installed Git ([git-scm.com](https://git-scm.com/downloads))  
  - Cloned Developer Training Course materials

### 16 June 2025
- Started setting up the CKB Dev Blockchain on Windows:  
  - Set up Tippy following [GitHub repository](https://github.com/nervosnetwork/tippy)  
  - Ran `./ckb list-hashes` in Windows PowerShell, got empty response

### 17 June 2025
- **Updated CKB Configuration Hashes**
  - Investigated why `./ckb list-hashes` returned no results.
  - Confirmed that syncing hadn’t yet completed, and that hash values must be manually retrieved.

  **Main Steps:**
  1. Extracted existing genesis block hash and code hash from the local `ckb.toml` and `specs/dev.toml`
  2. Cross-checked them with Tippy output logs
  3. Replaced the `genesis_hash` and `code_hash` in `ckb.toml` with the correct values
  4. Updated `tippy.toml` accordingly
  5. Restarted Tippy using updated configuration
  6. Validated successful start by confirming CKB node log output

  **Commands Used:**
  ```bash
  ./ckb list-hashes
  grep 'genesis' ~/.tippy/tippy.toml
  grep 'hash' ~/.tippy/tippy.toml
  grep -R "genesis" ~/.tippy
  grep -R "code_hash" ~/.tippy
  ./tippy restart
  ./tippy logs
  ```

  - This allowed proper setup of the local blockchain environment and hash-based configuration linking.

### 18 June 2025
- Installed VMware Workstation  
- Created a new virtual machine booted with Ubuntu to use Linux console alternative for the course

---

## Challenges & Notes
- Encountered empty response running `./ckb list-hashes` initially — solved by manually reviewing and updating the hash values from config and log files.
- Installation and blockchain setup required deep diving into configuration files and logs.

---

## Goals for Next Week
- Complete setup of full CKB dev chain and run smart contract lab exercises  
- Explore deeper Rust development  
- Start working through TypeScript-based dApp examples in Nervos training

---

*Report generated automatically using ChatGPT.*