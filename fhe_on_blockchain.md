FHE on blockchain
This section explains in depth the Zama Confidential Blockchain Protocol (Zama Protocol) and demonstrates how it can bring encrypted computation to smart contracts using Fully Homomorphic Encryption (FHE).

FHEVM is the core technology that powers the Zama Protocol. It is composed of the following key components.

- **FHEVM Solidity library**: Enables developers to write confidential smart contracts in plain Solidity using encrypted data types and operations.
- **Host contracts**: Trusted on-chain contracts deployed on EVM-compatible blockchains. They manage access control and trigger off-chain encrypted computation.
- **Coprocessors** – Decentralized services that verify encrypted inputs, run FHE computations, and commit results.
- **Gateway** – The central orchestrator of the protocol. It validates encrypted inputs, manages access control lists (ACLs), bridges ciphertexts across chains, and coordinates coprocessors and the KMS.
- **Key Management Service (KMS)** – A threshold MPC network that generates and rotates FHE keys, and handles secure, verifiable decryption.
