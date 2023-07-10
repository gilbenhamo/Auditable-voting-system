# Auditable Voting System

This repository contains an auditable voting application that ensures the confidentiality, integrity, and security of the voting process. It implements various cryptographic techniques such as zero-knowledge proofs, AES encryption and decryption, and ECDH key exchange. The system follows a client-server architecture where clients can participate in polls while maintaining the privacy of their votes. The voting data is stored in Excel sheets for easy auditing and verification.

## Features

- **Key Exchange with ECDH:** The system generates private and public keys for both the client and the server. Each side exchanges its public key to establish a shared key for secure communication.

- **Encryption with AES:** Clients can send their votes to the server securely. The server encrypts the votes using AES encryption and sends them back to the client. The client can decrypt the encrypted votes and verify their integrity.

- **Zero Knowledge Proof:** To ensure the validity of each vote, a unique token is generated for every vote cast. This token can be verified by entering it to the Committee for auditing purposes.

## Requirements
- Python 3.9 (or above)
- Make sure you have installed all the packages listed in the "requirements.txt" file.

## Usage
1. Clone the repository:
   ```shell
   git clone https://github.com/gilbenhamo/Auditable-voting-system.git
   cd auditable-voting-system
   ```

2. Install the required packages:
   ```shell
   pip install -r requirements.txt
   ```

3. Start the server:
   ```shell
   python Committee.py
   ```

4. Start the client:
   ```shell
   python VoteSystem.py
   ```

## Authors
- [Gil Ben Hamo](https://github.com/gilbenhamo)
- Itzik Rahamim
- Yovel Aloni
