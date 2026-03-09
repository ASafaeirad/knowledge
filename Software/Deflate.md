---
tags:
  - compression
  - cs
  - software
---
DEFLATE is a **lossless compression algorithm** that combines:
- [[LZ77]] (dictionary-based compression)
- [[Huffman coding]] (entropy coding)
It was designed by **Phil Katz** and is widely used in formats like **gzip, zlib, PNG, and ZIP**.

## How It Works
DEFLATE compresses data in two stages:
1. **LZ77 stage**
   - Finds repeated sequences in previously seen data
   - Replaces them with references (distance, length)
1. **[[Huffman coding]] stage**
   - Encodes the resulting symbols using variable-length codes
   - Frequently used symbols get shorter codes

Pipeline:

Raw Data → LZ77 Matching → Huffman Encoding → Compressed Output

## Data Blocks
DEFLATE stores compressed data in **blocks**.

Block types:
- Uncompressed block
- Fixed Huffman codes
- Dynamic Huffman codes

Dynamic blocks typically produce better compression.

## Key Properties
- Lossless compression
- Streaming-friendly
- Works well for text and structured data
- Fast decompression

## Important Notes
- DEFLATE itself does **not include headers or metadata**.
- It is often wrapped in container formats:
  - zlib
  - gzip
  - ZIP
- Compression ratio depends heavily on **repeated patterns**.
- Window size is typically **32 KB** for back-references.