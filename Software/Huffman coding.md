---
tags:
  - compression
  - cs
  - software
---
Huffman coding is a **lossless entropy encoding algorithm** created by **David A. Huffman in 1952**. It compresses data by assigning **shorter codes to frequent symbols** and **longer codes to rare symbols**.

## Core Idea
Instead of fixed-length encoding:
A = 8 bits

Huffman encoding:
A = 1  
B = 01  
C = 001  
D = 000  

Frequent symbols use fewer bits.

## Huffman Tree
![[HuffmanTree.png]]
Steps:
1. Count frequency of symbols
2. Build a binary tree from lowest frequency upward
3. Assign binary codes based on tree traversal

## Key Properties
- Prefix-free encoding
- No code is a prefix of another
- Allows unambiguous decoding

## Important Notes
- Huffman coding requires **symbol frequency statistics**.
- Two variants exist:
  - Static Huffman coding
  - Dynamic Huffman coding
- Often used after dictionary compression algorithms like [[LZ77]].
- Used in many compression systems:
  - [[DEFLATE]]
  - JPEG
  - MP3