# Cryptography

**Cryptography, or cryptology**, is the practice and study of techniques for secure communication in the presence of adversarial behavior. More generally, cryptography is about constructing and analyzing protocols that prevent third parties or the public from reading private messages.

**Cryptography** is the art of keeping information secure by transforming it into form that unintended recipients cannot understand. In cryptography, an original human readable message, referred to as plaintext, is changed by means of an algorithm, or series of mathematical operations, into something that to an uninformed observer would look like gibberish; this gibberish is called ciphertext.

### Modern cryptography concerns itself with the following four objectives:
1. **Confidentiality**. The information cannot be understood by anyone for whom it was unintended.
2. **Integrity**.The information cannot be altered in storage or transit between sender and intended receiver without the alteration being detected.
3. **Non-repudiation**. The creator/sender of the information cannot deny at a later stage their intentions in the creation or transmission of the information.
4. **Authentication**. The sender and receiver can confirm each other's identity and the origin/destination of the information.

## Cryptographic algorithms
Cryptosystems use a set of procedures known as cryptographic algorithms, or ciphers, to encrypt and decrypt messages to secure communications among computer systems, devices and applications.

A cipher suite uses one algorithm for encryption, another algorithm for message authentication and another for key exchange. This process, embedded in protocols and written in software that runs on operating systems (OSes) and networked computer systems, involves:

* public and private key generation for data encryption/decryption
* digital signing and verification for message authentication
* key exchange

## Types of cryptography
- **Single-key or symmetric-key encryption algorithms**
- **Public-key or asymmetric-key encryption algorithms**

## Caesar Cipher in Cryptography
The **Caesar Cipher** technique is one of the earliest and simplest methods of encryption technique. It’s simply a type of substitution cipher, i.e., each letter of a given text is replaced by a letter with a fixed number of positions down the alphabet. For example with a shift of 1, A would be replaced by B, B would become C, and so on. The method is apparently named after Julius Caesar, who apparently used it to communicate with his officials. 

## how computers generate random numbers
There are two main methods that a computer generates a random number: true random number generators (TRNGs) and pseudo-random number generators (PRNGs). The former uses some phenomenon outside the computer for its number generation, whereas the latter relies on pre-set algorithms to emulate randomness

