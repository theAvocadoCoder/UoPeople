Part 1

MV (2019) describes a programming paradigm as the framework that shapes how developers think about programming problems. They influence how programs are written, organized, and understood. Some of the most common paradigms are Structured, Functional, and Object-Oriented Programming.

Structured programming emphasizes sequence, selection, and iteration as the building blocks of control flow (Busbee & Braunschweig, 2018). This means that programs are organized into logical steps that flow predictably from one operation to the next. As Chaudhuri (2020) notes, this kind of structure allows for the visual representation of logic via flowcharts, improving clarity and debugging efforts.

This can be illustrated in a simple program to compute the average of numbers.
- Read input
- Calculate sum
- Divide by count
- Display result
Each step defined in the sequence performs a single task, making it easier to locate errors or modify the program.

Functional programming takes a more mathematical approach where all the code is executed within isolated functions. It focuses on pure functions, which have no side effects, always return the same result for the same input, and are not influenced by variables beyond their scope, making it easier to reason about programs (MV, 2019; Yatsko & Suslow, 2016).

The `map()` function in JavaScript or Python illustrates this perfectly. Instead of modifying values in place, `map()` returns a new list. This manifestation of immutability makes debugging more straightforward (Nduta, 2023) and allows for safer parallel processing, since no two functions compete to change the same data.

Object-Oriented Programming (OOP) organizes software around data types (Yatsko and Suslow, 2016). It mirrors how we understand real-world entities, making it ideal for modeling complex systems. Its core ideas are:
- abstraction and encapsulation: hides the internal workings of an object, exposing only what is necessary through methods or interfaces;
- inheritance: allows one class to build upon another; and
- polymorphism: enables multiple classes to share a common interface but behave differently when used.

A good example is a `Employee` class with subclasses like `Designer` and `Engineer`. Each subclass can calculate its salary differently, but they all share a method name like `getSalary()`. This makes the system flexible and extendable without changing existing code.


Part 2

There are seven phases in the lifecycle of software; the first two involve problem analysis and software design (Yatsko & Suslow, 2016; Charles Edeki, 2022). 

Designing a new software solution begins with problem analysis. Charles Edeki (2022) highlights the steps in this phase. First, I would determine an analysis strategy by studying the existing system. Relevant questions include: who is this software for, how will it be used, what data should the inputted or outputted, what actions should be restricted (Yatsko & Suslow, 2016)? Having these conversations with stakeholders would enable me to grasp the scope of the problem; this would form the basis of my software requirements specification (SRS).

Once the problem is defined, I will focus on how to structure the solution in the design phase. According to Yatsko and Suslow (2016), well-designed systems consider efficiency, reliability, and scalability from the start. To achieve this, I would apply abstraction and encapsulation to ensure modularity and code reusability. At this stage, I will use Unified Modeling Language (UML) diagrams to visualize how components interact. This ensures that failure or change of one module does not affect others.

Borrowing from functional programming, I would also consider using pure functions and immutable data structures in critical sections of the system. This approach allows me follow the single responsibility principle as well as the open-close principle. It also minimizes bugs related to shared state and makes debugging more predictable (Nduta, 2023). For applications handling concurrent tasks or sensitive data, this reduces the risk of hard-to-manage side effects and improves stability.

Word count (minus references and question): 620 words.

References

- Busbee, K. L., & Braunschweig, D. (2018). Structured programming. In Programming fundamentals: A modular structured approach using C++._ Rebus Community. [https://press.rebus.community/programmingfundamentals/chapter/structured-programming/](https://press.rebus.community/programmingfundamentals/chapter/structured-programming/)
- Charles Edeki. (2022, December 31). System Analysis: Systems Development Life Cycle (Planning, Analysis, Design and Implementation)_ [Video]. YouTube.
- Chaudhuri, A. B. (2020). Flowchart and algorithm basics: The art of programming._ Mercury Learning & Information.
- MV, T. (2019, November 12). What exactly is a programming paradigm?_ freeCodeCamp.org. [https://www.freecodecamp.org/news/what-exactly-is-a-programming-paradigm/](https://www.freecodecamp.org/news/what-exactly-is-a-programming-paradigm/
- Nduta, A. (2023, January 25). What is debugging? A simple guide for beginners_. CareerFoundry. [https://careerfoundry.com/en/blog/web-development/what-is-debugging/](https://careerfoundry.com/en/blog/web-development/what-is-debugging/)
- Yatsko, A., & Suslow, W. (2016). Insight into theoretical and applied informatics: Introduction to information technologies and computer science._ Walter de Gruyter GmbH.

Question: The most common design principles: single-responsibility principle, open-close principle, Liskov-substitution principle, interface-segregation principle, and dependency-inversion principle (SOLID) all come from the object-oriented programming paradigm. Does this imply that OOP is the most suitable paradigm for today's software landscape?

