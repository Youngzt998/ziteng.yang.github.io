---
layout: home
title: "PL&CS.Materials"
permalink: /study/
published: true
---



## **Public Materials for PL&CS Research/Study** 

(Extremely) slowly updating ...

Note1: All of those material's link are public on internet. They are collected based my personal interests. 

Note2: Some of them are picked from great Chinese language materials (described only in Chinese) for people studying in China.

### **Programming Languages (Research Oriented)**

#### **a. Basic Programming Language Theory**

- Formal Semantics: TODO
- Program Logic: TODO
- 



#### **b. Program Verification (Based on Proof Assistant )**

- The [*DeepSpec*](https://deepspec.org/main) project
- **Formal verification & basic PL theory based on proof assistant Coq:**
  - **[Foundations of proof assistant Coq]** Open-source free online-book *[**Software Foundations, Volume 1**](https://softwarefoundations.cis.upenn.edu/lf-current/index.html)*
  - **[Foundations of Hoare-Logic based program verification]**  ***[Software Foundations, Volume 2](https://softwarefoundations.cis.upenn.edu/plf-current/index.html)***
  - 
  - 
- **Formal verification - theoretical view**
  - **[Separation Logic & Verifiable C & Verified Compiler & CompCert Memory Model & ...]**  [**Program Logics for Certified Compilers**](https://vst.cs.princeton.edu/veric/) by Andrew W. Appel (free from author's page) 
  - Updating ...
- **Reading List: Compiler Verification (CompCert C compiler and its variants)**
  - **Original CompCert Compiler** (without linking or concurrency): 
    - [Leroy's Lectures & Slides](https://xavierleroy.org/courses/EUTypes-2019/),
    -  [Online Codes](https://compcert.org/doc/): [General Framework](https://compcert.org/doc/html/compcert.common.Smallstep.html), [Final Theorem](https://compcert.org/doc/html/compcert.driver.Compiler.html), [Clight(important simplification from C) and its semantics](https://compcert.org/doc/html/compcert.cfrontend.Clight.html), [RTL Optimizing IR](https://compcert.org/doc/html/compcert.backend.RTL.html)
  - **Language-Independent Linking (Difficult problem, difficult approach) **  : 
    - [POPL’15] Compositional CompCert
  - **Language-Independent Linking (Difficult problem, difficult approach)**: 
    - [POPL’15] Deep Specifications and Certified Abstraction Layers
  - **Same compiler linking (but lightweight proof)** 
    - [POPL’16] Lightweight verification of separate compilation
  - **Language-Independent Linking**: CompCertM
    - [POPL’20] CompCertM: CompCert with C-assembly linking and lightweight modular verification
    - Difficult problem, simpler approach
  - **Supporting Concurrency**: CASCompCert
    - [PLDI'19] Towards Certified Separate Compilation for Concurrent Programs
  - **Verified Translation Validator**:
    - [POPL'08] Formal verification of translation validators: a case study on instruction scheduling optimizations
    - [OOPSLA'19] Certified and efficient instruction scheduling: application to interlocked VLIW processors
    - [CPP'22] Formally verified superblock scheduling
- **Separation Logic - Basic**
  - Software Foundations, Volume 6
- **Separation Logic - Tools**
  - **VST [Verified Software Tool Chain] for C program**: ***[Software Foundations, Volume 5](https://softwarefoundations.cis.upenn.edu/vc-current/index.html)***

  - **Iris Project**: TODO




#### **c. Concurrency Theory**

TBD



#### **d. Parallel Programming**

- TODO
- Concurrency vs. Parallelism



#### **e. Program Analysis**

- **Static Analysis Foundations:**
  - An introduction online book [***Static Program Analysis*** ](https://cs.au.dk/~amoeller/spa/) by A. Møller and M. Schwartzbach,2018
  - Perfectly designed course slides from Nanjing University  [[course website](https://pascal-group.bitbucket.io/teaching.html)]

- Undecidability of Program Analysis: See Computability section below 
- **C**ontext **F**ree **L**anguage **Reachability for Static Analysis**: 
  - Read [**this paper**](https://dl.acm.org/doi/10.1145/199448.199462) from [POPL'95] to learn about **how some static analysis problem can be reduced to graph-reachability problem**
  - [Slides] TODO
  - 

- Static Analysis for Parallel Program



### **Theoretical Computer Science (Interests Oriented)**

#### **a. Computability**

- **Recursion Theory (Basic Computability)**
  - [Textbook] Computability: An introduction to recursive function theory
  - [Slides] TODO
- **Undecidable Problems**
  - Why Program Analysis is Undecidable: TODO
  - Rice Theorem: TODO

- 

#### **b. Computational Complexity**



#### **c. Algorithm**

- 



### **Logic & Foundation of Mathematics**

#### **a. Logic**

- First-order Logic
  - [Textbook] TODO
  - [Great Slides] TODO
- Modal Logic
  - [Textbook] TODO
  - [Great Slides] TODO

#### **b. Set Theory**

- TODO





### **Computer System (Courses Oriented)**

- Operating System
  - Course [MIT 6.S081](https://pdos.csail.mit.edu/6.S081/2020/schedule.html) and Labs from it
  -  [Xv6 Reference Book](https://pdos.csail.mit.edu/6.S081/2020/xv6/book-riscv-rev1.pdf) from 6.S081may be a better textbook for beginner's (than those famous books)
  - A Chinese Textbook: 上海交大软院的*[IPADS实验室](https://ipads.se.sjtu.edu.cn/)*实验室撰写的这本中文教材 [*《现代操作系统：原理与实现》*](https://ipads.se.sjtu.edu.cn/mospi/) 是计算机类中文教材中难得的写得较好的一本（个人阅读过大部分内容，认为不适合初学；但如果初学过一遍操作系统导论课程仍然觉得不知所云，可以解决很多的疑惑）


- Computer Architecture: TODO



### **$\alpha$. Tools**

- [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/) from MIT, including shells, git version control, vim editor, debugging tools, etc.

  [计算机教育中缺失的一课](https://missing-semester-cn.github.io/) (中文翻译版)，包括了shell窗口、git版本控制、vim编辑器、调试器等工具的使用

- Latex Cheating sheet [TODO]

- Linux shell Cheating sheet [TODO] 

- Git cheating sheet [TODO]



