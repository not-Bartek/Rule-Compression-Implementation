# Rules Compression

---

## Overview

This project focuses on compressing a set of rules from a file (`rules.txt`) into a smaller, more efficient set of rules while preserving their functionality. The goal is to optimize the representation of rules for better performance and storage efficiency.

---

## main.ipynb

The `main.ipynb` notebook contains the implementation of the rules compression process. The key steps are as follows:

1. **Loading the Rules**:
- The rules are loaded from the `rules.txt` file into a structured format for processing.

2. **Preprocessing**:
- Greek letters are changed to latin alphabet

3. **Prediction**:
- Rules are predicting labels on the given dataset then positive predictions are summed and divided by number of records to calculate the accuracy
- Then rules are simillarly tested on more specific datasets - one containing only old donors and one with only young to see if some rules aren't overspeciffic or too easy to satisfy.
4. **Compression**:
- Rules with accuracy less than 70% are removed
- mimimal accuracy of 70% is often used in statistics
5. **Output**:
- The final compressed rules are saved to a new file (`compressed_rules.txt`) for further use.

---

## Methods Used

 **Validation Metrics**:
- Ensures the compressed rules maintain the best rules based on accuracy.

---

## Author

Bartosz Dźwigała
