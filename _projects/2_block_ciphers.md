---
layout: page
title: Post-Quantum Block Ciphers
description: Analyzing block cipher security in the quantum era
img: assets/img/block-cipher.svg
importance: 2
category: research
related_publications: true
---

## Block Ciphers in the Post-Quantum Era

This project investigates the security of symmetric block ciphers against quantum adversaries, culminating in a publication in IEEE Xplore.

### Background

Block ciphers are fundamental building blocks of modern cryptography, used in:

- Data encryption (AES, DES)
- Authentication protocols
- Hash function constructions
- Key derivation functions

### Quantum Threat Analysis

**Grover's Algorithm Impact**

Grover's quantum search algorithm provides a quadratic speedup for searching unstructured databases. For block ciphers, this means:

$$\text{Effective key length} = \frac{n}{2}$$

where $n$ is the original key length.

| Cipher | Classical Security | Post-Quantum Security |
|--------|-------------------|----------------------|
| AES-128 | 128 bits | 64 bits |
| AES-192 | 192 bits | 96 bits |
| AES-256 | 256 bits | 128 bits |

### Key Findings

1. **Key Size Requirements**: To maintain current security levels, key sizes should be doubled
2. **Mode of Operation**: Some modes are more vulnerable than others
3. **Implementation Considerations**: Quantum resistance requires careful protocol design

### Publication

This work resulted in the IEEE publication:

> **A Review of Block Ciphers and Its Post-Quantum Considerations**
> *IEEE Xplore, 2024*
> [Read the paper](https://ieeexplore.ieee.org/abstract/document/10938619)

### Future Directions

- Analysis of emerging post-quantum symmetric primitives
- Hybrid classical-quantum security proofs
- Performance optimization for quantum-resistant implementations
