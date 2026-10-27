# Last-night sheet

Everything to read the evening before the exam: definitions, the protocol steps examiners look for, the formulas, and the numericals to rehearse once more.

## Definitions (underline these in the exam)

| Term | Definition |
|---|---|
| Cryptography / cryptanalysis | Keeping messages secure / breaking ciphertext; together: cryptology |
| Key space | Set of all possible keys; n bits → 2<sup>n</sup> keys |
| Substitution cipher | Each character replaced by another; positions kept |
| Transposition cipher | Characters kept; order permuted |
| One-time pad | Truly random key as long as the message, used once: unconditionally secure |
| Protocol | A series of steps, involving two or more parties, to accomplish a task |
| One-way function | Easy to compute, hard to reverse; trapdoor: easy to reverse with a secret |
| One-way hash function | Fixed-length h = H(M); pre-image, second pre-image and collision resistant |
| MAC | C(K, M): keyed checksum giving integrity + authentication (no non-repudiation) |
| Digital signature | Computed from the message hash with the private key; verified with the public key |
| Secret sharing (m, n) | n shares; any m recover the secret, m − 1 reveal nothing |
| Zero-knowledge proof | Proving knowledge of a secret without revealing it |
| Blind signature | Signer signs without seeing the content |
| Oblivious transfer | Receiver gets one of the secrets; sender does not know which |
| Key management | Generation, distribution, verification, storage, use, update, backup, revocation, destruction of keys |
| Nonlinear key space | Only keys built by a secret rule are strong; others give weak encryption |

## Lists examiners count

- **Cryptanalytic attacks:** ciphertext-only, known-plaintext, chosen-plaintext, adaptive chosen-plaintext, chosen-ciphertext, chosen-key, rubber-hose.
- **Four substitution types:** simple, homophonic, polygram, polyalphabetic.
- **Protocol characteristics:** known in advance, agreed, unambiguous, complete. **Types:** arbitrated, adjudicated, self-enforcing. **Attacks:** passive, active, cheaters.
- **Symmetric problems:** secret key distribution, compromise exposes all, n(n − 1)/2 keys.
- **Authentication function classes:** message encryption, MAC, hash function.
- **Signature requirements:** authentic, unforgeable, not reusable, unalterable, not repudiable.
- **Why sign the hash:** speed, short signature, stops RSA multiplicative forgery, separate storage, collision resistance.
- **ZKP properties:** completeness, soundness, zero-knowledge.
- **Secret sharing requirements:** threshold secrecy, correct reconstruction, verifiable shares, cheater detection, secure distribution, fresh randomness.
- **Contract signing versions:** arbitrator, face to face (letter by letter), probabilistic, cryptographic (OT + bit-by-bit release).
- **Key selection:** true randomness, full key space, adequate length, pass phrases/KDFs, X9.17, avoid weak keys, separate keys, limited lifetime.
- **KMS components:** generation, distribution, storage (HSM), access control, rotation, backup/escrow, revocation, destruction, audit.
- **Public-key distribution:** announcement, directory, authority, certificates.
- **Choosing an algorithm:** published, manufacturer, consultant, government, your own.
- **AES round:** SubBytes, ShiftRows, MixColumns, AddRoundKey (no MixColumns in the last round).

## Formulas

| Item | Formula |
|---|---|
| Caesar | C = (P + k) mod 26 |
| Vigenère | C<sub>i</sub> = (P<sub>i</sub> + K<sub>i</sub>) mod 26 |
| Hill | C = K × P mod 26; key valid if gcd(det K, 26) = 1; K<sup>−1</sup> = (det)<sup>−1</sup> × adj K |
| XOR / OTP | C = P ⊕ K, P = C ⊕ K |
| Diffie–Hellman | Y = α<sup>X</sup> mod q; K = Y<sub>B</sub><sup>X<sub>A</sub></sup> = Y<sub>A</sub><sup>X<sub>B</sub></sup> mod q |
| RSA | n = pq, φ = (p − 1)(q − 1), d = e<sup>−1</sup> mod φ; C = M<sup>e</sup> mod n, M = C<sup>d</sup> mod n |
| RSA blind | m′ = m·k<sup>e</sup>; s′ = m′<sup>d</sup>; s = s′·k<sup>−1</sup> (mod n) |
| Fiat–Shamir | v = s<sup>2</sup>; x = r<sup>2</sup>; y = r·s<sup>b</sup>; check y<sup>2</sup> = x·v<sup>b</sup> (mod n) |
| Shamir | f(x) = S + a<sub>1</sub>x + … (mod p); S = Σ y<sub>i</sub> Π x<sub>j</sub>/(x<sub>j</sub> − x<sub>i</sub>) |
| MAC tied to plaintext | E(K2, [M ‖ C(K1, M)]) |
| Sign then encrypt | E<sub>B</sub>(S<sub>A</sub>(M)) |
| 3DES (2 keys) | C = E<sub>K1</sub>(D<sub>K2</sub>(E<sub>K1</sub>(P))) |
| DES | 64-bit block, 56-bit key, 16 rounds, 8 S-boxes 6→4, subkeys 48 bits |
| AES | 128-bit block; 128/192/256-bit key; 10/12/14 rounds |

## The numericals: answers to check against

| Question | Answer |
|---|---|
| Playfair, NETWORK, INFORMATIONSECURITY (End Q2a) | DOIEKLGASCOLOKNDGOZY |
| Playfair, SECURE, HIDEGOLD (Mid-1 Q1) | IKBCBTKF |
| Playfair, MONARCHY, INSTRUMENTS | GATLMZCLRQXA |
| Columnar, NETWORK, INFORMATIONSECURITY (Mid-1 Q2) | NIRACXITURSYMEXFOIONT |
| Hill [[3,3,2],[2,5,1],[1,2,4]], SECUREDATATRANSFER (End Q4a) | SGIPZSVZBNICXFUJVD (det ≡ 5) |
| Hill [[2,4,5],[9,2,1],[3,17,7]], TOPGUN (Mid-1 Q5) | NGKBDH (det ≡ 21) |
| Hill [[3,3],[2,5]], HELP | HIAT |
| Vigenère, KEY, CRYPTOGRAPHY | MVWZXMQVYZLW |
| DH q = 41, α = 6, X<sub>A</sub> = 5, X<sub>B</sub> = 7 (End Q6a) | Y<sub>A</sub> = 27, Y<sub>B</sub> = 29, K = 38 |
| DH q = 7, α = 3, X = 2, 3 (Mid-2 Q5) | Y = 2, 6; K = 1 |
| DH q = 23, α = 5, X = 6, 15 | Y = 8, 19; K = 2 |
| RSA p = 17, q = 11, e = 7, M = 88 | d = 23, C = 11 |
| RSA p = 3, q = 11, e = 3, M = 4 | d = 7, C = 31 |
| Shamir p = 13, f(x) = 5 + 4x + 3x<sup>2</sup> | shares (1,12) (2,12) (3,5) (4,4) (5,9); S = 5 |

## Diagrams to practise once

1. Encryption model with key and Eve.
2. Playfair 5×5 square for NETWORK.
3. Arbitrated / adjudicated / self-enforcing protocols.
4. KDC key distribution (Alice, Trent, Bob, numbered arrows).
5. Hash-and-sign; sign-then-encrypt.
6. MAC tied to plaintext with K1 and K2.
7. Diffie–Hellman message flow; man-in-the-middle.
8. (3, 5) secret sharing.
9. ZKP cave.
10. Blind signature: blind → sign → unblind.
11. Contract signing with OT and bit-by-bit release.
12. Key life cycle; KMS components; four public-key distribution methods.
13. DES structure and f-function; AES round.

## The night-before plan

1. Read this sheet (40 minutes).
2. Do the NETWORK Playfair and the SECURE DATA TRANSFER Hill on paper without looking; check against the table.
3. Do the q = 41 Diffie–Hellman on paper.
4. Say aloud the answers to Mid-2's four theory questions (key management, KMS components, key space, key selection): they came back word for word last year.
5. Sleep. A rested brain writes 4–5 pages per question.
