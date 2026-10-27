# All past papers

Every MJPRU Network Security and Cryptography (CS-443T) question we could find, typed out and tagged by unit. The answer to every numerical is linked: they are all solved step by step in the unit notes.

::: warn Only three papers exist online
CS-443T is a new elective; no older MJPRU papers for it could be found (mjpruonline.com has none). This page has the three papers from our batch. If you have another paper, send it in and it will be added.
:::

## End-sem 2025-26 (paper code 23299)

**B.Tech (Seventh Semester) (Main/Back) Examination 2025-26 · CS-443T (CS & IT) · Network Security and Cryptography**<br>
Time: Three Hours · Maximum Marks: 70 · Attempt any five questions. All questions carry equal marks.

| Q | Question | Unit |
|---|---|---|
| 1 (a) | Explain the basic terminology used in cryptography. Discuss substitution and transposition ciphers in detail with examples. | 1 |
| 1 (b) | Discuss classical encryption techniques used in cryptography. Explain why they are insufficient for modern secure communication. | 1 |
| 2 (a) | Using the Playfair cipher, encrypt the plaintext "INFORMATION SECURITY" with the key "NETWORK". **[numerical]** | 1 |
| 2 (b) | Critically analyze the key distribution problem in symmetric key cryptography. Explain how public key cryptography and trusted third parties mitigate this issue, with suitable protocol-level justification. | 2 |
| 3 (a) | Describe the Advanced Encryption Standard (AES) in detail. Explain its encryption process with a neat block diagram. Also, analyze why AES is considered more secure and efficient than DES. | 5 (AES is beyond the syllabus) |
| 3 (b) | Discuss the role of cryptographic hash functions in digital signature schemes. Explain why signing the hash of a message is preferred over signing the message directly. | 2 |
| 4 (a) | Encrypt the plaintext "SECURE DATA TRANSFER" using the Hill Cipher technique. Use the key matrix [[3, 3, 2], [2, 5, 1], [1, 2, 4]]. **[numerical]** | 1 |
| 4 (b) | Explain the concept of Secret Sharing schemes. Discuss their security requirements and practical applications in distributed and fault-tolerant systems. | 3 |
| 5 (a) | What is a Zero-Knowledge Proof (ZKP)? Explain its fundamental properties. Also, analyze how blind signatures and oblivious signatures enhance privacy and anonymity in cryptographic protocols. | 3 |
| 5 (b) | Explain the protocol of Simultaneous Contract Signing. Discuss how cryptographic primitives such as zero-knowledge proofs and blind/oblivious signatures are used to ensure fairness and non-repudiation. | 3 |
| 6 (a) | Given a prime number q = 41 and a primitive root α = 6, demonstrate the correctness of the key exchange by verifying that both parties generate the same shared secret key using the algorithm. **[numerical]** | 3 |
| 6 (b) | Discuss the various strategies for cryptographic key selection. Analyze how improper key selection can compromise system security. | 4 |
| 7 (a) | Define Key Space in cryptography. Differentiate between linear key space and non-linear key space, highlighting their impact on cryptographic strength. | 4 |
| 7 (b) | What is meant by Key Management in cryptographic systems? Critically explain the mechanism of public key distribution and its associated challenges. | 4 |
| 8 | Write short notes on any **four**: (a) Cryptographic Protocols (b) Digital Signatures with Encryption (c) Nonlinear Key Space (d) Simultaneous Contract Signing (e) One-Time Pad (f) Public Key vs Symmetric Key Cryptography | 1–5 |

::: tip Answers to the numericals
- **Q2(a) Playfair, key NETWORK:** INFORMATIONSECURITY → **DOIEKLGASCOLOKNDGOZY** ([Unit 1](#unit1)).
- **Q4(a) Hill:** SECUREDATATRANSFER → **SGIPZSVZBNICXFUJVD** (C = K × P, A = 0) ([Unit 1](#unit1)).
- **Q6(a) Diffie–Hellman, q = 41, α = 6:** the private keys are not given, so choose them and say so. With X<sub>A</sub> = 5, X<sub>B</sub> = 7: Y<sub>A</sub> = 27, Y<sub>B</sub> = 29, shared key K = **38** ([Unit 3](#unit3)).
:::

## Mid-1 2025 (dated 08.10.2025)

**Department of CSIT · 1st Mid Semester Examination B.Tech (2025-26) · Cryptography and Network Security (CS-443T)**<br>
M.M. 10 · Time: 1 Hour · All questions are compulsory and carry equal marks.

| Q | Question | Unit | Came back in end-sem? |
|---|---|---|---|
| 1 | Use a Playfair cipher with the keyword SECURE to encrypt the message "HIDE GOLD". Show all steps clearly. | 1 | **Yes: Q2(a), new key and plaintext** |
| 2 | The transposition cipher is applied to the message "INFORMATIONSECURITY" using the keyword NETWORK. Construct the encryption matrix and find the ciphertext. | 1 | Yes: Q1(a) transposition |
| 3 | Explain the working of a symmetric cryptosystem using an appropriate diagram. Then, demonstrate how digital signatures and encryption can be integrated for secure communication. | 2 | Yes: Q8(b) short note |
| 4 | What do you mean by authentication function? Discuss MAC for authentication tied to plain text. | 2 | Close: Q3(b) hash in signatures |
| 5 | Encrypt the text "TOP GUN" using the Hill Cipher technique with the key [[2, 4, 5], [9, 2, 1], [3, 17, 7]]. | 1 | **Yes: Q4(a), new key and plaintext** |

Answers: Q1 → **IKBCBTKF**; Q2 → **NIRACXITURSYMEXFOIONT** (padded with X); Q5 → **NGKBDH**. All worked in [Unit 1](#unit1).

## Mid-2 2025 (dated 22.12.2025)

**Department of CSIT · IInd Mid Semester Examination B.Tech (2025-26) · Cryptography and Network Security (CS-443T)**<br>
M.M. 10 · Time: 1 Hour · Attempt any five questions.

| Q | Question | Unit | Came back in end-sem? |
|---|---|---|---|
| 1 | Define the Data Encryption Standard (DES). Describe its internal architecture and operational phases with the support of a block diagram. | 5 | Close: Q3(a) AES vs DES |
| 2 | What is meant by Key Management in cryptographic systems? Critically explain the mechanism of public key distribution and its associated challenges. | 4 | **Yes, word for word: Q7(b)** |
| 3 | Identify and explain the fundamental components of a cryptographic Key Management System (KMS). | 4 | Close: Q7(b) |
| 4 | Define Key Space in cryptography. Differentiate between linear key space and non-linear key space, highlighting their impact on cryptographic strength. | 4 | **Yes, word for word: Q7(a)** |
| 5 | Explain the Diffie–Hellman key exchange protocol. Mathematically verify the correctness of the shared secret generation for q = 7, X1 = 2, X2 = 3. | 3 | **Yes: Q6(a), new numbers** |
| 6 | Discuss the various strategies for cryptographic key selection. Analyze how improper key selection can compromise system security. | 4 | **Yes, word for word: Q6(b)** |

Answer to Q5: α was not given; with the primitive root α = 3, Y<sub>1</sub> = 2, Y<sub>2</sub> = 6 and K = **1**. (Any primitive root gives K = 1 here, because X1 × X2 = 6 = q − 1; worked in [Unit 3](#unit3).)

## Syllabus (CS-443T)

| Unit | Syllabus |
|---|---|
| 1 | **Introduction:** Terminology, Substitution ciphers and Transposition ciphers, Simple XOR, One-Time Pads, Computer Algorithms. Cryptographic Protocols. |
| 2 | **Protocol Building Blocks:** Introduction, Communication using Symmetric Cryptography, One-Way Functions, One-Way Hash Functions, Communication using Public-Key Cryptography, Digital Signatures, Digital Signatures with Encryption. |
| 3 | **Protocols:** Authentication and Key Exchange, Key Exchange, Authentication, Multiple-key public key cryptography, Secret splitting, Secret Sharing, Cryptographic protection. Zero-Knowledge Proofs, Zero-Knowledge Proofs of Identity, Blind Signatures, Oblivious Transfer, Oblivious Signature, Simultaneous contract signing, Cryptographic Techniques. |
| 4 | **Key Management:** Generating Keys, Nonlinear Keyspaces, Transferring Keys, Verifying Keys, Using Keys. |
| 5 | **Using Algorithms:** Choosing an Algorithm, Public-Key Cryptography versus Symmetric Cryptography, Encrypting Communication Channels, Encrypting Data for Storage. Cryptographic Algorithms: RSA, DES. |

**Books:** (1) *Applied Cryptography*, Bruce Schneier, John Wiley & Sons. (2) *Network Security and Cryptography*, William Stallings. (3) *Concept of Network Security and Cryptography*, Frozen. The syllabus follows Schneier's chapter titles almost exactly (chapters 1–3, 4–5, 8, 10), so Schneier is the main book.
