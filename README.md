# Statistical Fault Attack on AES

## Overview

This repository presents the implementation and analysis of a **Statistical Fault Attack (SFA)** against the AES block cipher. Statistical fault attacks exploit faults injected during cryptographic computations to recover secret information by analyzing the statistical properties of faulty ciphertexts.

The project demonstrates how implementation-level vulnerabilities can compromise the security of cryptographic systems despite the theoretical security of the underlying algorithm.

---

## Objectives

- Understand fault-based cryptanalysis of AES
- Analyze the effect of injected faults on AES computations
- Recover secret key information using statistical techniques
- Evaluate attack effectiveness under different fault models
- Study implementation security against fault injection attacks

---

## Background

Fault attacks are a powerful class of implementation attacks where an adversary deliberately induces errors during cryptographic operations.

Examples of fault injection techniques include:

- Voltage glitching
- Clock glitching
- Laser fault injection
- Electromagnetic fault injection
- Rowhammer-style memory faults

By comparing correct and faulty outputs, attackers can infer internal states and ultimately recover secret keys.

---

## AES Overview

| Parameter | Value |
|------------|---------|
| Cipher | AES-128 |
| Block Size | 128 bits |
| Key Size | 128 bits |
| Number of Rounds | 10 |

The attack targets vulnerabilities introduced by faulty intermediate computations rather than weaknesses in the AES algorithm itself.

---

## Methodology

1. Generate correct AES ciphertexts.
2. Inject faults during encryption.
3. Collect faulty ciphertext samples.
4. Perform statistical analysis on fault distributions.
5. Identify exploitable leakage patterns.
6. Recover candidate key information.

---

## Features

- AES implementation and evaluation
- Fault injection simulation
- Statistical analysis of faulty outputs
- Key recovery techniques
- Experimental validation of attack feasibility
- Visualization of fault distributions

---

## Security Implications

This project highlights the importance of:

- Fault detection mechanisms
- Redundant computation
- Error-correcting techniques
- Secure hardware design
- Side-channel resistant implementations

---

## Applications

The concepts explored in this repository are relevant to:

- Embedded security
- Hardware security
- Cryptographic engineering
- Secure processor design
- Smart cards
- IoT security
- Side-channel and fault analysis research

---

## Technologies Used

- Python
- NumPy
- Cryptographic Analysis
- Statistical Methods

---

## Results

The implemented attack demonstrates how statistically analyzing faulty ciphertexts can reveal information about secret AES key material under realistic fault models.

---

## Author

Bhavya Dixit  
