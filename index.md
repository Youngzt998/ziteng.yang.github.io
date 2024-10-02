---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: ""
---

# **Biography** 

I am a PhD student in the [PLSE Lab](https://www.scs.gatech.edu/content/programming-languages-software-engineering) at **[Georgia Institute of Technology (GT)](https://www.gatech.edu/)** since 2021, advised by Prof. [**Vivek Sarkar**](https://vsarkar.cc.gatech.edu/). My current research area are **program logic & verification**, **parallelism & concurrency**, and their application in compilers. 

Before joining Georgia Tech, I spent my undergraduate time at **[Shanghai Jiao Tong University (SJTU)](https://www.sjtu.edu.cn/)**, major in [Computer Science](http://www.cs.sjtu.edu.cn/en/).  I was advised by Prof. **[Qinxiang Cao](https://jhc.sjtu.edu.cn/people/members/faculty/qinxiang-cao.html)** and worked on ***compiler correctness*** and ***mathematical logic*** in the ***Coq proof assistant*** from junior to senior year. Prior to that I studied in Prof. **[Xiang Yin](http://xiangyin.sjtu.edu.cn/)**'s' group and worked on **Automata Theory** (specifically, *supervisory control* of *Discrete Event System*) during sophomore year.

I'm open to internship. Here is my **[CV](./cv/CV_ZitengYang.pdf)**.

**Contact Information:**

- **Email Address (Institution):**  (fun x y => x dot y @gatech.edu) ziteng yang
- **Physical Address:** ~~0C-DD-24-F6-DE-9C~~ [Klaus Advanced Computing Building](https://www.scs.gatech.edu/content/building-facilities), room 2319
- [Twitter](https://twitter.com/_ziteng_yang_), [LinkedIn](https://www.linkedin.com/in/ziteng-yang-a149181b5/)

# **Research**

My current major focus (PhD Thesis) is on improving certified compilation. In the mean time, I also pay attention to the area of parallelism & concurrency, computability theory etc. See the detailed problems I'm investigating below:

**Program Logic & Certified Compilation** (major)

- **[Ongoing] Verified Linear Scan Register Allocation**: Implementing an alternative register allocation algorithm in a formally verified compiler instead of graph-coloring algorithm that has both lightweight time complexity and verification burden.
- **[Ongoing] Improving the Correctness Theory of Certified Compiler**: Fixing a "missing correctness specification" of in the correctness of CompCert framework.
- **[[Published](./papers/oopsla24/oopslab24-final.pdf)] Verified Instruction Scheduling**: Achieved the first ever fully verified instruction scheduling passes in a formally verified compiler
- Q: How do we improve the general framework for CompCert to make a parallelizing compilation (e.g. Parallelizing loops in GCC -O3 optimization)
- Q: How do we ensure that the formal semantics specification of C (source language) and assembly/machine language (target language) is correct w.r.t. their language design?
- Q: How could equality saturation be used to improve a certified compiler optimization?
- Q: How to implement inter-procedural optimizations in a certified compiler? Is current general framework enough?

**Parallelism & Concurrency** (secondary)

- **[Ongoing] Program Analysis on Data-race problems**: Investigating some better approaches on both static prediction and dynamic detection of data-races.

**Computability view of Program Verification and Analysis** (in spare time)

- Q: How do we establish a theory in computability view for [*annotation verifier*](https://dl.acm.org/doi/10.1145/3632911) (programs annotated with its verification)



**Undergraduate Researches**

- **Compiler Correctness for Annotation Verifier** [Advised by [Qinxiang Cao](https://jhc.sjtu.edu.cn/people/members/faculty/qinxiang-cao.html)]: 
  
  I worked on investigating correctness theory of compiling programs annotated with verification information ([*annotation verifier*](https://dl.acm.org/doi/10.1145/3632911)) and using them as optimization hints. I proposed an extended semantic and verification framework and gave a trial on toy language/logic. 
  
  This expedition was continued by [Hanzhi Liu](https://scholar.google.com/citations?user=hEUk48QAAAAJ), [Yanning Chen](https://lightquantum.me/), etc. to go beyond toy language using my framework.
  
- **Supervisor Control of Timed Discrete-Event Systems** [Advised by [Xiang Yin](http://xiangyin.sjtu.edu.cn/)]: Investigated the supervisory control problem for timed discrete-event systems (TDES) under partial observation where time was considered as a special event.

# **Publications**

<u>Program Verification:</u>

- **Ziteng Yang**, Jun Shirako, Vivek Sarkar, Fully Verified Instruction Scheduling, OOPSLA’24 [[PDF](./papers/oopsla24/oopslab24-final.pdf)]

<u>Automata Theory:</u> 

- **Ziteng Yang**, Xiang Yin and Shaoyuan Li. “Maximally permissive supervisor control of timed discrete-event systems under partial observation,” in 21st IFAC World Congress, 2020.  [ [PDF](./papers/IFAC2020/IFAC2020-Final-Full.pdf)  l  [Slide](./papers/IFAC2020/IFAC2020-Slides.pdf) l  [Video Report (Youtube)](https://youtu.be/GtbxR_OKfXU) ]. 

# **Teaching Experience**

- **Teaching Assistant** for *CS6390@GT: Programming Languages*, 2023 spring, taught by [**Vivek Sarkar**](https://vsarkar.cc.gatech.edu/)
  - The foundational principles of programming languages

- **Teaching Assistant** for *CS4510@GT: Automata and Complexity*, 2022 fall, taught by [Joseph Jaeger](https://faculty.cc.gatech.edu/~josephjaeger/)
  - Intro to Compatibility: regular language and DFA/NFA, context-free language and PDA, Turning Machine, P/NP/co-NP., L/NL, co-NL 
- **Teaching Assistant**  for *MA208@SJTU: Discrete Mathematics (IEEE/AI Honor Class)*, 2020 fall, taught by [Qinxiang Cao](http://jhc.sjtu.edu.cn/people/members/qinxiang-cao.html) .
  - First-order Logic (proof, semantics and soundness), Set Theory as foundation of Mathematics

- **Teaching Assistant** for  *MA239@SJTU: Discrete Mathematics (Zhiyuan Honor Class)*, 2020 fall, taught by [Xiang Yin](http://xiangyin.sjtu.edu.cn/).
  - Logic and deduction, Graph Theory, Set Theory

# **Honors and Scholarships**

**During PhD Program**

- **Conference Travel Grant** by scholarship of PLMW@PLDI’22, San Diego, Jun. 2022

**During Undergraduate Time**

- **Rongchang Scholarship for Science and Technology Innovation, Finalist** (20 persons school-wide each  year; **10,000 CNY**) , Oct. 2020
  
  **荣昶科技创新奖学金, 提名奖 (人民币壹万元)**

- **Undergraduate Excellent Scholarship, Third-class** (Top 20%; **500 CNY**), Oct. 2018
  
  **上海交通大学校优奖学金, C等 (人民币伍佰元)**

  

# **Misc**

- My hometown is [Chongqinq](https://youtu.be/yzl4jc9E5GU?si=DSd5Imm1ZIIlUgCE), the [Night City](https://cyberpunk.fandom.com/wiki/Night_City) of China. Do pay a visit.
- I'm a cat person. Here's [my cat](https://youngzt998.github.io/mycat/).
- I love playing tennis so much that it hurts my scaphoid bone accidentally : (

