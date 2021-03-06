# Frequent Pattern Mining
This question aims to provide you a better understanding of the frequent pattern mining and the closed/maximal pattern mining.
1. Implement a frequent pattern mining algorithm (e.g., the Apriori algorithm or FP- Growth) to mine the frequent patterns from a transaction dataset.
2. Implement a closed pattern mining algorithm to mine the closed frequent patterns from the same transaction dataset. An easy way is to write code based on the frequent patterns you got from part 1.
3. Implement a maximal pattern mining algorithm to mine the maximal frequent patterns from the same transaction dataset. An easy way is to write code based on the frequent patterns you got from part 1.

## Specification:
- The frequent patterns should be ordered according to their support from largest to small- est. Ties should be resolved by ordering the frequent patterns according to the alphabetical order.
- First print all the frequent patterns for part 1, then the closed frequent patterns for part 2 and last the maximal frequent patterns for part 3. Each part should be separated by an empty line.
- Please refer to the sample output below. In sample output 0, the first 9 patterns are the frequent patterns for part 1, the following 3 patterns are the closed frequent patterns for part 2 and the last 2 patterns are the maximal frequent patterns for part 3.

## Input Format
- The input dataset is a transaction dataset.
- The first line of the input corresponds to the minimum support.
- Each following line of the input corresponds to one transaction. Items in each transaction are separated by a space.

Please refer to the sample input below. In sample input 0, the minimum support is 2, and the dataset contains 3 transactions and 5 item types (A, B, C, D and E).

## Constraints
NA

## Output Format
- The output are the frequent patterns you mined out from the input dataset.
- Each line of the output should be in the format:

    Support [ frequent pattern ]

    Support [ frequent pattern ]

    ......

### Sample Input 0
	2
	B A C E D
	A C
	C B D

### Sample Output 0
	3 [C]
	2 [A]
    2 [A C]
    2 [B]
    2 [B C]
    2 [B C D] 2 [B D]
    2 [C D]
    2 [D]
    
    3 [C]
    2 [A C]
    2 [B C D]
    
    2 [A C]
    2 [B C D]

### Sample Input 1
	2
	data mining
	frequent pattern mining
	mining frequent patterns from the transaction dataset 
	closed and maximal pattern mining

### Sample Output 1
    4 [mining]
    2 [frequent]
    2 [frequent mining] 
    2 [mining pattern] 
    2 [pattern]
    
    4 [mining]
    2 [frequent mining]
    2 [mining pattern]
    
    2 [frequent mining]
    2 [mining pattern]


## Dependencies
- None

## Requirements
- Python 3

## Run as
	python PatternMining.py
