# 4-mer Sequence Reconstruction

This repository contains a Python script that reconstructs a linear string by concatenating a list of 4-mers (substrings of length 4). The goal is to take a set of 4-mers and merge them into a continuous string, which is often a part of sequence assembly tasks in bioinformatics.

## Problem Overview

Given a list of 4-mers, such as ["AAAT", "AATG", "ACCC", "ACGC"], the task is to:
1. Concatenate all the 4-mers into a single, continuous linear string.
2. This reconstructed string represents a potential sequence derived from smaller k-mers.

## Script

```python
# Define the composition of 4-mers
composition = [
    "AAAT", "AATG", "ACCC", "ACGC", "ATAC", "ATCA", "ATGC",
    "CAAA", "CACC", "CATA", "CATC", "CCAG", "CCCA", "CGCT",
    "CTCA", "GCAT", "GCTC", "TACG", "TCAC", "TCAT", "TGCA"
]

# Create the linear string by concatenating the 4-mers
linear_string = "".join(composition)

# Print the linear string
print(linear_string)
```
Example Output

AAATAATGACCCACGCATACATCAATGCCAAACACCCATACATCCCAGCCCACGCTCTCAGCATGCTCTACGTCACTCATTGCA

Requirements
Python 3.6 or higher

No external libraries are required.

Applications
Bioinformatics sequence assembly

K-mer based string reconstruction

Genome assembly tasks

License
This project is released under the MIT License.


