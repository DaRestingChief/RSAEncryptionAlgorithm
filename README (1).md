#  RSA Encryption & Decryption (From Scratch)

This project demonstrates a **complete implementation of the RSA Cryptosystem** using pure Python — without relying on cryptography libraries. The goal is to clearly show how public and private keys are generated and how real text is encrypted and decrypted using modular arithmetic.

---

##  What This Project Shows

- Generating **two large prime numbers**
- Computing **n = p × q** and **φ(n)** (Euler’s Totient)
- Selecting **public key (e)** such that `gcd(e, φ(n)) = 1`
- Computing **private key (d)** using modular inverse
- Encrypting a message using:

  \[
  c = m^e \mod n
  \]

- Decrypting using:

  \[
  m = c^d \mod n
  \]

All of this is done in about **60 lines of readable Python**, making the cryptographic logic transparent and easy to follow.

---

##  Why a Simple Implementation?

This implementation intentionally avoids:
- Miller–Rabin primality testing  
- Extended Euclidean Algorithm  
- High-level crypto libraries  

**Reason:**  
The aim here is *clarity over optimization*.  
This code is best suited for **learning, teaching, and demonstration purposes**, where each step should be visible and understandable.

---

##  How to Run

```bash
python main.py
