---
tags:
  - compression
  - cs
  - software
---
## Overview
Entropy coding is a **lossless compression technique** that encodes symbols using **variable-length codes based on their frequency**.

The idea comes from **information theory**, where entropy measures the **minimum number of bits needed to represent information**.

Frequent symbols require fewer bits, while rare symbols require more bits.

## Example
Symbol frequencies:
```
A → 50%  
B → 25%  
C → 15%  
D → 10%
```

Possible encoding:
```
A = 0  
B = 10  
C = 110  
D = 111
```
Frequent symbols use shorter codes, reducing the total size.

## Purpose
Entropy coding removes **statistical redundancy** from data. In modern compression systems it is often used **after another compression step**.

## Common Entropy Coding Algorithms
- [[Huffman Coding]]
- Arithmetic Coding
- Range Coding
## Key Properties
- Lossless compression
- Based on probability of symbols
- Produces variable-length bit sequences
- Approaches theoretical compression limits

## Important Notes
- Entropy coding works best when symbol frequencies vary widely.
- It does **not detect repeated patterns**, other algorithms like [[LZ77]] do that.
