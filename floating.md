# Testing Differential Privacy Systems for Floating-Point Vulnerabilities: A Black-Box Approach  

## Status 

    - Available
    - Level: master thesis 

## Company 

[DPella AB](www.dpella.io) is a deep tech startup that has developed a solution
to do privacy preserving analytics using Differential Privacy (DP) technology
(see below). DPella’s team of world experts (all with PhDs) in DP technology and
in building privacy-by-design and secure-by-design systems believe that this
technology is the best existing approach for doing privacy preserving analytics.  

- DPella AB supervisor: Marco Gaboardi  
- Chalmers supervisor: Prof. Alejandro Russo
- Possible examiner: Prof. David Sands

## Proposal 

[Differential privacy](https://link.springer.com/chapter/10.1007/11681878_14)
(DP) is a widely adopted framework for protecting the privacy of individuals in
datasets while enabling the release of statistical insights. The DP mechanism
relies heavily on adding carefully calibrated noise, such as Laplace or
Gaussian noise, to analytical results. While DP is theoretically robust, its
practical implementation often depends on floating-point arithmetic,
introducing vulnerabilities that can compromise privacy guarantees.

Two prominent attacks have demonstrated these vulnerabilities:  

1. **[Mironov's Floating-Point Attack
   (2010)](https://www.microsoft.com/en-us/research/wp-content/uploads/2012/10/lsbs.pdf):**
   This attack reveals how deterministic noise patterns can emerge due to the
   limited precision of floating-point arithmetic.  

2. **[Precision-Based Attack
   (2022)](https://tpdp.journalprivacyconfidentiality.org/2022/papers/HaneyDHSH22.pdf):**
   This recently identified issue, detailed by Tumult Labs, underscores
   additional risks stemming from floating-point inaccuracies.  

Despite the clear need for secure DP systems, there is no standardized
framework or test suite to evaluate their resilience against these
floating-point vulnerabilities. As organizations increasingly adopt DP systems,
the lack of such a tool poses significant risks.

### **Expected Outcomes**  
1. **A Comprehensive Test Suite:**  An open-source **Haskell-based tool** capable
   of identifying floating-point vulnerabilities in DP systems.  

2. **Documentation and Guidelines:**  Detailed instructions for using the tool,
   along with guidelines for organizations to mitigate identified
vulnerabilities.  

3. **Case Studies:**  Practical demonstrations of the test suite’s capabilities
   through evaluations of popular DP libraries.  

4. **Contribution to the Community:**  By open-sourcing the tool, this project
   will enable widespread adoption and foster collaboration to improve the
reliability of DP systems.  


## Related work 

- [Are We There Yet? Timing and Floating-Point Attacks on Differential Privacy
Systems](https://ieeexplore.ieee.org/document/9833672)

- [Preserving differential privacy under finite-precision
semantics](https://inria.hal.science/hal-01390927/document)

## What would you learn by doing this project? 

- **Differential Privacy Fundamentals**  
  - Understanding the theoretical basis of Differential Privacy, its
  guarantees, and its implementation challenges.  

  - Exploring mechanisms like Laplace and Gaussian noise addition and their
  vulnerability to floating-point inaccuracies.  

- **Floating-Point Arithmetic**  
  - Gaining insights into how floating-point arithmetic works in computer
  systems.  

  - Studying known vulnerabilities in floating-point arithmetic, such as
  Mironov's attack and precision-based attacks.  

- **Black-Box Testing Techniques**  
  - Designing and implementing a black-box testing framework to evaluate DP
  systems.  

- **Programming in Haskell**  
  - Developing modular, extensible, and reusable components for the test suite.  


