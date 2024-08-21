---
title: "CMPT 125 Intro. to CS & Programming II"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/cmpt125
venue: "Simon Fraser University, School of Computing Science"
date: 2023-01-01
location: "Burnaby/Surrey, BC, Canada"
---

An continuation from [CMPT 120](/_teaching/cmpt120.md) on programming and some CS-related concepts (e.g., history, problem-solving). Introduces students to some common data structures (e.g., stacks, queues, linked lists, trees) and algorithms (e.g., Mergesort, Quicksort). C and C++ are the programming languages of choice.

**This is for reference only. For actual outline refer to the course webpage at Canvas (our LMS).**
Content is subject to change (plus I often update it). This is the schedule I used for Spring 2023.

Course Description
======
A rigorous introduction to computing science and computer programming, suitable for students who already have some background in computing science and programming. Intended for students who will major in computing science or a related program. Topics include: fundamental algorithms; elements of empirical and theoretical algorithmics; abstract data types and elementary data structures; basic object-oriented programming and software design; computation and computability; specification and program correctness; and history of computing science.

Course Objectives
======
This course introduces students to fundamental concepts of computing science and programming. By the end of the course, students will be familiar with building blocks of a computer program such as variables, arrays, pointers, recursions; as well as higher level concepts such as analysis of algorithms and coding style. Students will gain valuable knowledge and experience by solving problems using computational thinking.

By the end of this course students should be able to:
* Design and implement solutions to problems using C/C++
* Explain, analyze, and compare algorithms in terms of performance
* Describe and utilize fundamental computing science concepts such as data structures
* Maintain good coding practice and style

Recommended Textbooks
======
Seacord, R. C. (2020). Effective C. In Effective C. No Starch Press. [Online access](https://sfu-primo.hosted.exlibrisgroup.com/permalink/f/1u29dis/TN_cdi_proquest_ebookcentral_EBC6180065) (requires SFU login)
<br />
Stroustrup, B. (2024). Programming : principles and practice using C++ / Bjarne Stroustrup. (Third edition.). Addison-Wesley. [Online access](https://sfu-primo.hosted.exlibrisgroup.com/permalink/f/usv8m3/01SFUL_ALMA51493802270003611) (requires SFU login)

Course Schedule
======

| Week  | Topics | Readings/Watchings[^1]                                       |
| ----- | ------ | ------------------------------------------------------------ |
| 1     | Course intro {::nomarkdown}<ul><li>Logistics, expectations</li><li>Intro to C, Coding Environments</li></ul>{:/} | Effective C chapters: 1 |
| 2     | C basics (Part 1) {::nomarkdown}<ul><li>Variables & strong typing</li><li>Data vs address</li><li>Pointers, references, arrays</li><li>Constant variabes</li><li>Strings</li><li>Reading from stdin</li><li>2D arrays</li></ul>{:/} | Effective C chapters: 2 & 5 |
| 3     | C basics (Part 2) {::nomarkdown}<ul><li>Composite datatypes & enums</li><li>Functions, return values, & conditions</li><li>Global & static variables</li><li>Macros</li><li>Memory allocation</li><li>Execution stack</li></ul>{:/} | Effective C chapters: 2 & 5, 6 |
| 4     | C basics (Part 3) {::nomarkdown}<ul><li>Returning structs, pointers to functions</li><li>Binary encoding of numbers</li><li>Pseudo-code</li><li>Recursion</li><li>Algorithms & performance</li></ul>{:/} | Learn more about sorting with visualization {::nomarkdown}[<a href="https://visualgo.net/bn/sorting">LINK</a>]{:/} |
| 5     | Basic algorithms & data structures (Part 1) {::nomarkdown}<ul><li>Big-O notation</li><li>Searching algorithms</li></ul>{:/} | Learn more about searching with visualization {::nomarkdown}[<a href="https://www.cs.usfca.edu/~galles/visualization/Search.html">LINK</a>]{:/} |
| 6     | Basic algorithms & data structures (Part 2) {::nomarkdown}<ul><li>Sorting algorithms</li></ul>{:/}<br />Abstract data types| Learn more about sorting with visualization {::nomarkdown}[<a href="https://visualgo.net/bn/sorting">LINK</a>]{:/} |
| 7     | Basic algorithms & data structures (Part 3) {::nomarkdown}<ul><li>Stacks</li></li>Queues</li></ul>{:/} | External readings: {::nomarkdown}<ul><li><a href="https://www.programiz.com/dsa/stack">Stacks</a></li><li><a href="https://www.programiz.com/dsa/queue">Queues</a> (note that their use of the rear index is different from the lectures)</li><li><a href="https://www.programiz.com/dsa/linked-list">Linked lists</a></li></ul>{:/} |
| 8     | Reading break | - |
| 9     | Basic algorithms & data structures (Part 4) {::nomarkdown}<ul><li>Linked lists</li></ul>{:/}<br />Recursion revisited | - |
| 10    | Basic algorithms & data structures (Part 5) {::nomarkdown}<ul><li>Intro to graphs & trees</li><li>Tree traversals & operations</li></ul>{:/} | Additional references to {::nomarkdown}<a href="https://www.programiz.com/dsa/trees">Trees</a>{:/} |
| 11    | Basic algorithms & data structures (Part 6) {::nomarkdown}<ul><li>Binary Search Trees (BSTs)</li></ul>{:/} | Learn more about BSTs with visualization {::nomarkdown}[<a href="https://visualgo.net/en/bst">LINK</a>]{:/} |
| 12    | Intro to C++ (Part 1) {::nomarkdown}<ul><li>cin/cout</li><li>strings</li><li>function overloading</li><li>templates</li></ul>{:/} | External readings: {::nomarkdown}<ul><li><a href="https://www.programiz.com/cpp-programming/input-output">cin/cout</a></li><li><a href="https://www.programiz.com/cpp-programming/strings">strings</a></li><li><a href="https://www.programiz.com/cpp-programming/function-overloading">function overloading</a></li><li><a href="https://www.programiz.com/cpp-programming/templates">tempaltes</a></li></ul>{:/} |
| 13    | Intro to C++ (Part 2) {::nomarkdown}<ul><li>Pass-by-reference functions</li><li>Operator overloading</li><li>Exception handling</li><li>Intro to OOP</li></ul>{:/} | Additional references: {::nomarkdown}<ul><li><a href="https://www.programiz.com/cpp-programming/constructors">constructors</a></li><li><a href="https://en.cppreference.com/w/cpp/language/operators">operator overloading</a></li></ul>{:/} |
| 14    | Intro to C++ (Part 3) {::nomarkdown}<ul><li>Object-Oriented Design (OOD)</li><li>Examples in C++</li></ul><br />Review{:/} | - |
| ??    | Final Exam   | - |

[^1]: References in Topics/Readings are for reference only. If there is any topic/concept that is in conflict between class slides and any of these references, what is taught in the classes will be used.
