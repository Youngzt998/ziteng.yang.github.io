---
layout: home
title: "Projects"
permalink: /project/
---




# **Research Projects**

## **Verification-aided Compiler Optimization**

We are considering a new method of program optimization for C programs with annotation that contains the verification information of the program.  A conditional definition of "forward simulation" and "backward simulation"  for compiler correctness was proposed with crucial properties proved formally in Coq. The new methods was being realized based on [CompCert](http://compcert.inria.fr/) compiler. We also implemented a translation path from annotated CompCert C source language to annotated RTL intermediate language. 

Further details are confidential currently.





## **Formalization of Completeness Proof of Propositional Dynamic Logic in Coq **

[UnifySL](https://github.com/QinxiangCao/UnifySL) is a library of the proof assistant [Coq](https://coq.inria.fr/) for logic under development (not open sourced for now). Formalized proof theories, semantic definitions, soundness proofs and completeness proofs of minimum logics, propositional logics and separation logics were realized using Coq's type classes and high-order features. The completeness proof of previous logics are all based on the framework of infinite canonical model.

My work aimed to investigate the finite model methods, starting the exploration from the formalizing of propositional dynamic logic (PDL), including the proof theories, semantic definitions, the proof of its soundness and  the proof of its weak completeness, making the best of framework and tools in UnifySL. Currently the completeness proof was finished, and we expect to extract a new framework of high-order abstraction for finite model methods in the future. 

During my work, a lot of useful lemmas was also proved as a supplementary of the UnifySL library. 



The following are the critical definitions and lemmas:

- The abstract type class of PDL

  ```
  Class Program : Type:={
    program: Type;
  }.
  
  Class PropositionalDynamicLanguage (L:Language)(Pro: Program):Type:={
    boxp: program -> expr -> expr
  }.
  
  Class ProgramOperation (L:Language)(Pro:Program):Type:= {
    choice: program -> program -> program;
    composition: program -> program -> program;
    iteration: program -> program;
    test: expr -> program
  }.
  ```

- The deep-embedded syntax of PDL

  ```
  Inductive program {Sigma: PropositionalVariables}{ProV: ProgramVariables}: Type :=
    | choice: program -> program -> program
    | composition: program -> program -> program
    | iteration: program -> program
    | test: expr -> program
    | basep: BaseP -> program
  with
   expr {Sigma: PropositionalVariables} {ProV: ProgramVariables}: Type :=
    | impp : expr -> expr -> expr
    | orp : expr -> expr -> expr
    | andp: expr -> expr -> expr
    | falsep : expr
    | boxp: program -> expr -> expr
    | varp : Var -> expr
  .
  ```

  

- The *Truth Lemma* and *Existence Lemma* (two mutually inductive lemmas):

  ```
  Lemma TRUTH_LEMMA:
    forall (psi x: exp) m Phi,
      rel psi m Phi -> 
        FL_closure_construction psi x ->
          (KRIPKE: canonical_Kmodel psi, m |= x <-> proj1_sig Phi x)
  with EXISTENCE_LEMMA:
    forall (pi: prog)(psi x: exp)(m : Kworlds (canonical_Kmodel psi)),
      FL_Atom psi (proj1_sig m) -> 
        FL_closure_construction psi ([pi]x) ->
          (proj1_sig m ([pi]x) <-> forall n, R_D pi m n -> proj1_sig n x).
  ```

  

-  The *Weak Completeness* Theorem

  ```
  Theorem complete_weakly: weakly_complete GP SM (KripkeModelClass _ kMC).
  ```








## **Supervisor Control of Timed Discrete-Event Systems **

The supervisory control theory of Discrete Event Systems (DES) is a formal framework for the synthesis of control logic for complex automated systems. We investigate the supervisory control problem for timed discrete-event systems (TDES) under partial observation where time was considered as a special event. The design objective is to synthesize a maximally-permissive supervisor to restrict the behavior of the system such that the closed-loop language is within a safe specification language. Relevant paper was accepted by [IFAC2020](https://www.ifac2020.org/),  see Publications.
We also hope to investigate the non-blocking problem employing nondeterministic control method in the future.

![avatar](./papers/IFAC2020/example.png)







# **Other Projects**

- **SimPL Interpreter**: an interpreter for a simple programming language called *SimPL*, implemented in **2020**.

- **Naive-Airdrop**: an application for encrypted file synchronization between PC and Android under the same wi-fi, implemented in **2019**.  

  (Both my first project using Java and first practical project for real life.)

- **In The Garden**: a mini puzzle game (Chinese version only), created in **2018**, with other two partner. 

  (My first mini-project of game design.)

- **Re-implementation of *deque* and *map* of  C++ Standard Template Library (STL)**: Re-implement the data structure *deque* (using Block List) and *map* (using AVL Tree) of C++ Standard Library, simulating most of their original designed functions, implemented in **2018**. 

  (My first project of programming.)

