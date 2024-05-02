# Rivest–Shamir–Adleman (RSA) Algorithm

RSA is a public-key cryptosystem that is widely used for secure data transmission. It was invented by Ron Rivest, Adi Shamir, and Leonard Adleman in 1977.

## Description

The RSA algorithm involves generating a pair of keys: a public key and a private key. The public key can be freely distributed and is used for encryption, while the private key is kept secret and is used for decryption.

The security of RSA relies on the difficulty of factoring large prime numbers. The algorithm works as follows:

1. **Key Generation**: 
    - Choose two distinct prime numbers, p and q.
    - Compute n = pq.
    - Compute φ(n) = (p-1)(q-1).
    - Choose an integer e such that 1 < e < φ(n) and gcd(e, φ(n)) = 1. This is the public exponent.
    - Compute d such that ed ≡ 1 (mod φ(n)). This is the private exponent.

2. **Encryption**:
    - To encrypt a message M, compute C ≡ M^e (mod n), where C is the ciphertext.

3. **Decryption**:
    - To decrypt the ciphertext C, compute M ≡ C^d (mod n), where M is the original message.

## Usage

This repository contains implementations of the RSA algorithm in various programming languages. You can use these implementations for educational purposes or integrate them into your projects where secure data transmission is required.

## Contributing

Contributions to this repository are welcome. If you have improvements or additional implementations of the RSA algorithm, feel free to open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

