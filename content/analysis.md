# PYQ analysis: what MJPRU actually asks

Three MJPRU CS-443T papers analysed: the 2025-26 end-sem, Mid-1 (08.10.2025) and Mid-2 (22.12.2025). With so few papers, the strongest signal is how the end-sem reused the mids.

::: tip The one-line summary
**The end-sem was built from the two mids.** Three Mid-2 questions came back word for word (key space, key management and public-key distribution, key selection). Mid-2's Diffie–Hellman came back with new numbers; Mid-2's DES came back as "AES, and why it beats DES". Mid-1's Playfair and Hill numericals came back with new keys. Learn every mid question, practise the three numericals (Playfair, Hill, Diffie–Hellman) until they are automatic, and add Unit 3's protocols (secret sharing, ZKP, contract signing).
:::

## Topic frequency (how many of the 3 papers asked it)

| Rank | Topic | Unit | Asked in | Count | Chance this year |
|---|---|---|---|---|---|
| 1 | **Playfair cipher numerical** | 1 | Mid-1 Q1, End Q2(a) | 2 / 3 | Very high |
| 2 | **Hill cipher numerical (3×3 key)** | 1 | Mid-1 Q5, End Q4(a) | 2 | Very high |
| 3 | **Key management + public key distribution** | 4 | Mid-2 Q2, Q3; End Q7(b) (same words) | 2 | Very high |
| 4 | **Key space: linear vs nonlinear** | 4 | Mid-2 Q4; End Q7(a), Q8(c) (same words) | 2 | Very high |
| 5 | **Key selection strategies, poor keys** | 4 | Mid-2 Q6; End Q6(b) (same words) | 2 | Very high |
| 6 | **Diffie–Hellman numerical** | 3 | Mid-2 Q5; End Q6(a) | 2 | Very high |
| 7 | **Terminology, substitution and transposition (columnar numerical)** | 1 | Mid-1 Q2; End Q1(a), Q1(b) | 2 | Very high |
| 8 | **DES architecture; AES vs DES** | 5 | Mid-2 Q1; End Q3(a) | 2 | High |
| 9 | **Digital signatures with encryption; symmetric cryptosystem** | 2 | Mid-1 Q3; End Q8(b) | 2 | High |
| 10 | **Hash functions in signatures; authentication functions and MAC** | 2 | Mid-1 Q4; End Q3(b) | 2 | High |
| 11 | **Simultaneous contract signing** | 3 | End Q5(b), Q8(d) | 1 | High |
| 12 | **Zero-knowledge proofs; blind and oblivious signatures** | 3 | End Q5(a) | 1 | High |
| 13 | **Secret sharing (and splitting)** | 3 | End Q4(b) | 1 | High |
| 14 | **Key distribution problem; KDC and public key** | 2 | End Q2(b) | 1 | Medium-high |
| 15 | One-time pad; public key vs symmetric; cryptographic protocols | 1, 5 | End Q8 (short notes) | 1 | Medium |
| — | **Not yet asked:** XOR, computer algorithms, one-way functions, authentication protocols (Needham–Schroeder, Kerberos, passwords and salt), multiple-key public key, oblivious transfer, transferring / verifying / using keys, choosing an algorithm, encrypting channels and storage, RSA | 1–5 | never | 0 | Medium: expect 2–3 of these |

```mermaid
flowchart LR
  A[Unit 1<br/>~25% of marks] --- B[Unit 2<br/>~15%]
  B --- C[Unit 3<br/>~25%]
  C --- D[Unit 4<br/>~20%]
  D --- E[Unit 5<br/>~10%]
```

## Unit-wise weight (2025-26 end-sem, 16 parts of 7 marks)

| Unit | Questions | Marks (of 112 on paper) |
|---|---|---|
| Unit 1 · Ciphers and protocols | Q1(a), Q1(b), Q2(a), Q4(a) | 28 |
| Unit 2 · Protocol building blocks | Q2(b), Q3(b) | 14 |
| Unit 3 · Advanced protocols | Q4(b), Q5(a), Q5(b), Q6(a) | 28 |
| Unit 4 · Key management | Q6(b), Q7(a), Q7(b) | 21 |
| Unit 5 · Using algorithms | Q3(a) | 7 |
| Mixed short notes | Q8 (any four of six) | 14 |

You need only 5 of 8 questions. **Units 1, 3 and 4 give 6 of the 8 questions**: get those three units and the numericals solid and you can choose comfortably.

## The numericals (the fastest full marks)

| Numerical | Asked | Answer on this site |
|---|---|---|
| Playfair, key SECURE, HIDE GOLD | Mid-1 Q1 | IKBCBTKF |
| Playfair, key NETWORK, INFORMATION SECURITY | End Q2(a) | DOIEKLGASCOLOKNDGOZY |
| Columnar transposition, key NETWORK, INFORMATIONSECURITY | Mid-1 Q2 | NIRACXITURSYMEXFOIONT |
| Hill, key [[2,4,5],[9,2,1],[3,17,7]], TOP GUN | Mid-1 Q5 | NGKBDH |
| Hill, key [[3,3,2],[2,5,1],[1,2,4]], SECURE DATA TRANSFER | End Q4(a) | SGIPZSVZBNICXFUJVD |
| Diffie–Hellman q = 7, X1 = 2, X2 = 3 | Mid-2 Q5 | K = 1 (with α = 3) |
| Diffie–Hellman q = 41, α = 6 | End Q6(a) | K = 38 (with X<sub>A</sub> = 5, X<sub>B</sub> = 7) |

All are solved step by step in [Unit 1](#unit1) and [Unit 3](#unit3). **Write your convention in the first line** (Hill: C = K × P with column vectors, A = 0; columnar: key letters ranked alphabetically, padding X; Diffie–Hellman: state the private keys you chose).

## Repeat-question patterns

- **Mid-2 is a preview of the end-sem.** Three of its six questions came back unchanged. When your Mid-2 paper arrives, treat every question on it as a likely end-sem question.
- **Numericals return with new numbers.** Playfair, Hill and Diffie–Hellman each appeared in a mid and again in the end-sem. Expect them again; Vigenère, rail fence and RSA are the natural next ones.
- **Long, "critically analyse" wording** in Units 2–4 ("critically analyze the key distribution problem…", "analyze how improper key selection…"). These want: definition, mechanism, a diagram, then a list of weaknesses or attacks and how they are fixed.
- **Short notes (Q8)** were "any four of six", so each is worth 3.5 marks: about one page.

## Predicted end-sem 2026-27 (most likely 8 questions)

| Q | (a) | (b) |
|---|---|---|
| 1 | Terminology; substitution vs transposition; why classical ciphers fail | Columnar / rail-fence numerical, or XOR and one-time pad |
| 2 | Playfair numerical | Hill numerical |
| 3 | Key distribution problem; communication using symmetric and public-key cryptography | One-way hash functions; digital signatures; signatures with encryption |
| 4 | Diffie–Hellman numerical; key exchange protocols (man-in-the-middle, interlock) | Authentication: passwords, salt, challenge–response, Needham–Schroeder / Kerberos |
| 5 | Secret splitting and secret sharing (Shamir) | Zero-knowledge proofs; ZKP of identity |
| 6 | Blind signatures, oblivious transfer and oblivious signatures | Simultaneous contract signing |
| 7 | Key space (linear vs nonlinear); generating keys and key selection | Key management: transferring, verifying, using keys; public-key distribution |
| 8 | DES (and AES vs DES); RSA; choosing an algorithm; encrypting channels and storage — or short notes | |

**Mock Paper 1** on this site is built on this prediction.
