# Some Notes on Code-Based Cryptography

## Abstract
This thesis presents new cryptanalytic results in several areas of coding- based cryptography. In addition, we also investigate the possibility of using convolutional codes in code-based public-key cryptograph. The first algorithm that we present is an information-set decoding algorithm, aiming towards the problem of decoding random linear codes. We apply the generalized birthday technique to information-set decoding, improving the computational complexity over previous approaches. Next, we present a new version of the McEliece public-key cryptosystem based on convolutional codes. The original construction uses Goppa codes, which is an algebraic code family admitting a well-defined code structure. In the two constructions proposed, large parts of randomly generated parity checks are used. By increasing the entropy of the generator matrix, this presumably makes structured attacks more difficult. Following this, we analyze a McEliece variant based on quasi-cylic MDPC codes. We show that when the underlying code construction has an even dimension, the system is susceptible to, what we call, a squaring attack. Our results show that the new squaring attack allows for great complexity improvements over previous attacks on this particular McEliece construction. Then, we introduce two new techniques for finding low-weight polynomial multiples. Firstly, we propose a general technique based on a reduction to the minimum-distance problem in coding, which increases the multiplicity of the low-weight codeword by extending the code. We use this algorithm to break some of the instances used by the TCHo cryptosystem. Secondly, we propose an algorithm for finding weight-4 polynomials. By using the generalized birthday technique in conjunction with increasing the multiplicity of the low-weight polynomial multiple, we obtain a much better complexity than previously known algorithms. Lastly, two new algorithms for the learning parities with noise (LPN) problem are proposed. The first one is a general algorithm, applicable to any instance of LPN. The algorithm performs favorably compared to previously known algorithms, breaking the 80-bit security of the widely used p512, 1 q 8 instance. The second one focuses on LPN instances over a polynomial ring, when the generator polynomial is reducible. Using the algorithm, we break an 80-bit security instance of the Lapin cryptosystem.

## Table of Contents

1.  Introduction
	1.1  Outline
	1.2  Notation
	1.3  Probability Theory and Combinatorics
	1.4  Information Theory
	1.5  Hypothesis Testing
	     1.5.1  The Walsh Transform
	1.6  Algorihms and Complexity Theory
	1.7  The Birthday Paradox and Collision Search
	     1.7.1  Searching For Collisions in Vector Spaces
	1.8  Cryptography and Cryptanalysis
	     1.8.1  One-way Functions
		 1.8.2  Symmetric Cryptography
		 1.8.3  Public-key Cryptography
		 1.8.4  Attack Models and Settings
		 1.8.5  Distinguising Attacks
	1.9 Summary

2.  Linear Codes
	2.1  General
	2.2  Channel Error Models
	2.3  Types of Decoding
	2.4  Random-Coding Bounds and Covering Codes
	2.5  Computational Problems and Coding
	2.6  Efficiently Decodable Families
	     2.6.1  Convolutional Codes
		 2.6.2  Cyclic Codes
		 2.6.3  Hamming Codes
		 2.6.4  LDPC and MDPC Codes
	2.7  Summary

3.  Information-Set Decoding
	3.1 Plain ISD and Lee-Brickell's Algorithm
	3.2 Stens's algorithm
	3.3 A New Algorithm
		3.3.1  Explaining the Ideas Behind the Algorithm
		3.3.2  Compleity Analysis
		3.3.3  Parameters and Security
	3.4  Summary

4. Code-Based Cryptography
	4.1  McEliece Cryptosystem
		4.1.1  The Original McEliece Construction
	4.2  Attacks in Code-Based Cryptography
	4.3  New Variants of McEliece Cryptosystems
		4.3.1  McEliece Based on Convolutional Codes
		4.3.2  McEliece Basedon MDPC codes
	4.4  The TCHo Cipher
		4.4.1  Proposed Parameters
	4.5  Summary

5.  A Squaring Attack on QC-MDPC-based McEliece
	5.1  A Key-Recovery Attack
		5.1.1  Polynomial Square Roots
		5.1.2  The Attack
	5.2  A Message-Recovery Attack
	5.3  Analysis
	5.4  Results
	5.5  Summary

6. Searching for Low-Weight Polynomial Multiples
	6.1  The Low-Weight Polynomial Multiple Problem
		6.1.1  Time-Memory Trade-off Approach
		6.1.2  Finding Minimum-Weight Codewords in a Linear Code
	6.2  A New Algorithm Solving LWPM
		6.2.1  Complexity Analysis
		6.2.2  Simulation Results
		6.2.3  The Attack
	6.3  A New Algorithm for Finding a Weight-4 Multiple
		6.3.1  Complexity Analysis
		6.3.2  Simulation Results
	6.4  Attacks on QC-MDPC McEliece in Relation to LWPM
	6.5  Summary
	
7.  Learning Parity with Noise
	7.1  The LPN Problem
	7.2  The BKW Algorithm
		7.2.1  LF1 and LF2 Variants
	7.3  A New Algorithm
		7.3.1  A Toy Example
	7.4  Algorithm Description
		7.4.1  Gaussian Elimination
		7.4.2  Merging Columns
		7.4.3  Partial Secret Guessing
		7.4.4  Covering-Coding Method
		7.4.5  Subspace Hypothesis Testing
	7.5  Analysis
	7.6  Results
		7.6.1  Lapin with an Irreducible Polynomial
	7.7  More on the Covering-Coding Method
	7.8  Summary

8.  LPN over a Polynomial Ring
	8.1  The Ring-LPN Problem
		8.1.1  Formal Definition
	8.2  A New Algorithm for Ring-LPN with Reducible Polynomial
		8.2.1  A Low-Weight Code from the CRT Map
		8.2.2  Using Low-Weight Relations to Build a Distinguisher
		8.2.3  Recovering the Secret Polynomial
	8.3  Lapin Authentication Protocol
	8.4  The Improved Version for the Proposed Instance of Lapin
	8.5  Complexity Analysis
	8.6  Results
	8.7  Summary
	
9.  Concluding Remarks
10.  References
		 