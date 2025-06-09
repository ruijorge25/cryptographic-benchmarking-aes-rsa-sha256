# cryptographic-benchmarking-aes-rsa-sha256
Benchmarking the performance of AES, RSA, and SHA-256 in Python through encryption, decryption, and hashing tests across multiple file sizes and environments

Cryptographic Benchmarking: AES, RSA, and SHA-256 Performance Comparison

This project presents a detailed analysis of the performance of three key cryptographic algorithms: AES (symmetric encryption), RSA (asymmetric encryption), and SHA-256 (hash function). It measures and compares their efficiency in terms of encryption, decryption, and hashing time across different file sizes and environments.

🔍 Objective
To evaluate and compare the computational performance of AES, RSA, and SHA-256 using Python implementations. Tests were performed on files of increasing sizes, with and without randomness, to assess consistency, scalability, and efficiency.

⚙️ Technologies Used

Python 3.13.2

Jupyter Notebook

Libraries: cryptography, hashlib, time, timeit, statistics, matplotlib, numpy, os, random

🧪 Methodology

Data Generation:

Simulated random files of various sizes

Organized in dictionaries for structured access

Algorithm Implementation:

AES: Mode CTR, 256-bit keys

RSA: Raw RSA, 2048-bit keys, no padding

SHA-256: Standard hashlib implementation

Performance Testing:

Each operation repeated 100 times for statistical relevance

Measured encryption/decryption/hash time using timeit

Statistical Analysis:

Compared average times using line plots

Created boxplots for variance and outlier analysis

Tested on two distinct hardware environments to verify consistency

📈 Results Summary

Algorithm: AES
Best Use Case: Bulk encryption
Strength: Speed and stability
Weakness: Slight performance drop with very large files

Algorithm: RSA
Best Use Case: Secure key exchange
Strength: Strong security
Weakness: High computational cost (especially for decryption)

Algorithm: SHA-256
Best Use Case: Data integrity
Strength: Fast and reliable
Weakness: Slightly slower on large files

See the HTML report (relatorio_comparativo_final.html) for full results and visual comparisons.

📂 File Structure

SP#1.ipynb: Main notebook with implementation and analysis

relatorio_comparativo_final.html: Interactive report with plots

SP#1.docx: Detailed academic report

data/: Folder with original input files

README.md: Project overview and instructions

🚀 How to Run

Clone the repository:
git clone https://github.com/ruijorge25/cryptographic-benchmarking-aes-rsa-sha256.git

Install the required libraries:
pip install cryptography matplotlib numpy

Launch the notebook:
jupyter notebook SP#1.ipynb

Run all cells to reproduce the tests and results

📌 Notes

For accurate benchmarking, close background applications and use high-performance mode

Two distinct machines were used to verify results under different CPU generations (i7-12700H vs i7-13620H)

📚 References

Python Docs: os, timeit, statistics, hashlib

cryptography.io

SSLDragon blog on AES vs RSA

numpy.org and matplotlib.org

Handbook of Applied Cryptography
