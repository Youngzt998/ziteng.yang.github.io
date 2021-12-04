---
layout: home
title: "Projects"
permalink: /project/
---






# **Research Projects**

## **Verification-aided Compiler Optimization**



[Note: This project was now continued by  [Hanzhi Liu](https://misaka.center/), an undergraduate genius student (2019~2023, expected) and an experienced programmer at SJTU, also advised by Qinxiang Cao, to implement this optimization and framework in VST's separation logic [VST = Verified Software Toolchain]]

We are designing a new method of program optimization for C programs with assertion annotated that contains verification information of the program. The new methods was being realized based on original [CompCert](http://compcert.inria.fr/) compiler. New semantics framework was designed based on CompCert small step semantic framework.  A conditional definition of "forward simulation" and "backward simulation" diagram for compiler correctness was proposed with crucial properties proved.

This is an original work of our research group under exploration, so details are still not opened to the public.





## **Finite Canonical Model for Completeness Theory in Coq Based on UnifySL**:

[UnifySL](https://github.com/QinxiangCao/UnifySL) is a library of the proof assistant [Coq](https://coq.inria.fr/) designed for basic mathematical logic (e.g. Propositional Logics, Separation Logics etc.) under development (not open sourced for now). Formalized proof theories, semantic definitions, soundness proofs and completeness proofs were abstractly described using Coq's type classes and high-order features. The completeness proof of previous logics are all based on the framework of infinite canonical model.

My work as a research assistant aimed to investigate the finite model methods, starting the exploration from the formalizing of propositional dynamic logic (PDL), including the proof theories, semantic definitions, the proof of its soundness and  the proof of its weak completeness, making the best of framework and tools in UnifySL. Currently the completeness proof was finished, and we expect to extract a new framework of high-order abstraction for finite model methods in the future. 

During my work, a lot of useful lemmas was also proved as a supplementary of the UnifySL library. 






## **Supervisor Control of Timed Discrete-Event Systems**

The supervisory control theory of Discrete Event Systems (DES) is a formal framework for the synthesis of control logic for complex automated systems. We investigated the supervisory control problem for timed discrete-event systems (TDES) under partial observation where time was considered as a special event. The design objective is to synthesize a maximally-permissive supervisor to restrict the behavior of the system such that the closed-loop language is within a safe specification language. Relevant paper was accepted by [21st IFAC World Congress, 2020](https://www.ifac2020.org/).
We also hope to investigate the non-blocking problem employing nondeterministic control method in the future.



The following figure illustrates our main process of synthesizing such safe and maximally permissive supervisory. 

![avatar](./papers/IFAC2020/example.png)

Here is our [video report](https://youtu.be/GtbxR_OKfXU) at [IFAC2020](https://www.ifac2020.org/) uploaded to YouTube.





---





# **Projects for Courses/Fun** 

[**Naive-Airdrop**](https://github.com/Youngzt998/Naive-Airdrop) 

- An application for encrypted file synchronization between PC and Android under the same wi-fi.  

- Features: auto connection, changes detecting of the observed files on client devices, encryption in transfer, both auto transmission and manual transmission etc.

- My design of the working logic of this application

  ![avatar](./projects/airdrop/structure.png)

---

[**SimPL Interpreter**](https://github.com/Youngzt998/SimPL-Interpreter): an interpreter for a simple programming language called *SimPL*,  a simplified dialect of *ML*, including *type checking* (including let-polymorphism) and *evaluation*.

- Examples of  SimPL

  - Recursive combinator:

    ```ocaml
    let gcd = rec g => fn a => fn b =>
                if b=0 then a else g b (a % b)
    in  gcd 34986 3087
    end
    (* ==> 1029 *)
    ```

  - Let-polymorphism: 

    ```ocaml
    let a = fn x => x in 
        let b = a 1 in 
            let c = a false in 
                if c then b else 0
            end
        end
    end
    (* ==> 0 *)
    ```
  
  
  

---

[**Linux (Android) Memory Management**](https://github.com/Youngzt998/Operating-System-Projects/tree/master/2)  

- Replacement of the original page replacement algorithm with a new one in a given specification.
-  See a detailed instruction (also a report) for beginner of (Linux) Operating System kernel investigation [here](./projects/os-prj-linuxmm/Instruction.pdf).



---

[**Re-implementation of *deque* and *map* of  C++ Standard Template Library (STL)**:](https://github.com/Youngzt998/Re-implementation-of-deque-and-map) Re-implement the data structure *deque* (using Block List) and *map* (using AVL Tree) of C++ Standard Library, simulating most of their original designed functions. 



