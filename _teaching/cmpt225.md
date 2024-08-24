---
title: "CMPT 225 Data Structures & Programming"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/cmpt225
venue: "Simon Fraser University, School of Computing Science"
date: 2024-05-01
location: "Burnaby/Surrey, BC, Canada"
---

One of the most important courses in the CS program. In SFU this is a pre-requisite course for over 20 CMPT courses and it is for good reasons: it teaches some of the most fundamental concepts in CS (e.g., abstract data types, algorithms, data structures) that are used in many advanced CS topics; it also teaches some programming techniques so students can comfortably implement those concepts and write their own programs. C++ is the programming language of choice (some versions use Java, goal is to have some form of OOP).

It is not an easy course and there are many things to cover (things ramp up very quickly after the first month). But a student who successfully completes this course will have the basic skillset to take on many other more complex CS subjects. My goal is to train students to have the mindset of a computer scientist and be able to both apply CS concepts to problem-solving, and appreciate the ideas behind those concepts.

**This is for reference only. For actual outline refer to the course webpage at Canvas (our LMS).**
Content is subject to change (plus I often update it). This is the schedule I used for Summer 2024.

![an image of the tentative course schedule](/images/cmpt225_tentativeCourseSchedule.jpg)

Course Description
======
Introduction to a variety of practical and important data structures and methods for implementation and for experimental and analytical evaluation. Topics include: stacks, queues and lists; search trees; hash tables and algorithms; efficient sorting; object-oriented programming; time and space efficiency analysis; and experimental evaluation.

Course Objectives
======
This course explores fundamental algorithms and data structures that can help in developing elegant and efficient solutions to complex problems. We will study their specification, analysis, implementation (in C++), evaluation, and applications. Platform: Linux (Ubuntu) Language: C++.

By the end of this course students should be able to:
* Design and implement solutions to problems using C++
* Explain, analyze, and compare algorithms in terms of performance
* Describe and utilize fundamental computing science concepts such as data structures
* Maintain good coding practice and style

Recommended Textbooks
======

* (DSA-C++ Book) Goodrich, M. T., Tamassia, R., & Mount, D. M. (2011). Data structures and algorithms in C++ (Second edition.). Wiley. [Online access](https://sfu-primo.hosted.exlibrisgroup.com/permalink/f/15tu09f/01SFUL_ALMA51324254930003611) (requires SFU login)
* Carrano, Henry, & Henry, Timothy. (2017). Data abstraction & problem solving with C++ : walls and mirrors / Frank M. Carrano, University of Rhode Island, Timothy M. Henry, New England Institute of Technology. (Seventh edition.). Pearson.
* Stroustrup, B. (2024). Programming : principles and practice using C++ / Bjarne Stroustrup. (Third edition.). Addison-Wesley. [Online access](https://sfu-primo.hosted.exlibrisgroup.com/permalink/f/usv8m3/01SFUL_ALMA51493802270003611) (requires SFU login)

Course Schedule
======

| Week  | Topics | Readings/Watchings[^1]                                       |
| ----- | ------ | ------------------------------------------------------------ |
| 1     | {::nomarkdown}Course intro<br />C++ primer<ul><li>Basic elements & expressions</li></ul>Coding environments{:/} | DSA-C++ Book: Ch. 1.1, 1.2 |
| 2     | C basics {::nomarkdown}<ul><li>Variables</li><li>Loops</li><li>Functions</li><li>I/O</li></ul>{:/} | DSA-C++ Book: Ch. 1.3, 1.4 |
| 3     | C with OOP {::nomarkdown}<ul><li>Classes</li><li>Inheritance</li><li>Operator overloading</li><li>Libraries & templates</li></ul>{:/} | DSA-C++ Book: Ch. 1.5-1.8, Ch. 2.1-2.3 |
| 4     | {::nomarkdown}Basic data structures<ul><li>Stacks & queues</li><li>Linked lists (singly & doubly)</li></ul>Execution Stacks & Recursions{:/} | DSA-C++ Book: Ch. 5.1-5.2, Ch. 3.2-3.3 |
| 5     | Basic algorithms (Part 1) {::nomarkdown}<ul><li>Big-O notation</li><li>Master theorem</li><li>Faster integer multiplication</li></ul>{:/} | DSA-C++ Book: Ch. 4.1-4.2 |
| 6     | Basic algorithms (Part 2) {::nomarkdown}<ul><li>Sorting algorithms</li><li>Binary Trees & Binary Search Trees</li></ul>{:/} | DSA-C++ Book: Ch. 11.1-11.3 (Sorting), Ch. 7.1-7.3 (BTs & BSTs) |
| 7     | Review & midterm | - |
| 8     | More data structures (Part 1) {::nomarkdown}<ul><li>Self-balancing BSTs</li><ul></li>AVL trees</li><li>2-3 trees</li><li>B-trees</li></ul></ul>{:/} | DSAC-C++ Book: Ch. 10.1-10.2, 10.4 (in this course I suggested my students to refer to the code covered in the lectures/labs) |
| 9     | More data structures (Part 2) {::nomarkdown}<ul><li>Priority queues</li><li>Heaps</li></ul>{:/} | DSA-C++ Book: Ch. 8 |
| 10    | More data structures (Part 3) {::nomarkdown}<ul><li>Graphs</li><ul><li>BFS & DFS</li><li>Dijkstra's & A* algorithms</li></ul></ul>{:/} | DSA-C++ Book: Ch. 13.1-13.5 (in this course I suggested my students to refer to the code covered in the lectures/labs) |
| 11    | More data structures (Part 4) {::nomarkdown}<ul><li>Hasing</li><ul><li>Separate chaining</li><li>Open addressing/probing</li><li>...and related topics</li></ul></ul>{:/} | DSA-C++ Book: Ch. 9.2 (in this course I suggested my students to refer to the code covered in the lectures/labs) |
| 12    | More data structures (Part 5) {::nomarkdown}<ul><li>Selection algorithms</li><li>Union-Find</li><li>Kruskal's algorithm</li></ul>{:/} | DSA-C++ Book: Ch. 11.4-11.5 |
| 13    | More algorithms {::nomarkdown}<ul><li>Evaluating arithmetic expressions</li><ul><li>Using recursion</li><li>Using stack</li><li>Using stack on prefix notation</li><li>Using recursion on expression tree</li></ul></ul>Review{:/} | - |
| ??    | Final Exam   | - |

[^1]: References in Topics/Readings are for reference only. If there is any topic/concept that is in conflict between class slides and any of these references, what is taught in the classes will be used.

Handy Online References
======

* Supplementary explanations of C++ [[LINK](https://www.programiz.com/cpp-programming/)]
* Supplementary descriptions of DSA [[LINK](https://www.programiz.com/dsa/)]
* Helpful visualization of algorithms [[LINK](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html)]
* Another helpful visulization of algorithms [[LINK](https://visualgo.net/)]