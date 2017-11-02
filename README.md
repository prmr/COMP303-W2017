# Introduction to Software Design with Java

This textbook provides an in-depth introduction to software design, with a focus on object-oriented design, and using the Java programming language. Compared with other resources for learning software design, this material is intended to have the following features:

* **Concrete:** The concepts presented are worked down to a level where they are directly applied in source code. For this reason, a minimum level of Java programming proficiency is necessary. It is important to note that the Java programming language is the learning tool that allows me to illustrate and discuss various design concepts: it is not the subject being taught. Learning software design in-depth requires the use of a programming language, but the knowledge gained is expected translate easily to other languages. This being said, we might as well choose a mature, free, and well-supported language. Translation of the material to use [Plankalk&uuml;l](https://en.wikipedia.org/wiki/Plankalk%C3%BCl) is left as an exercise.
* **Narrative:** This text follows a narrative style that links design problems, concepts, and solutions into a cohesive package. This is in contrast to reference material such as design pattern catalogs or API documentation.
* **Foundational:** *To the extent possible*, this material attempts to be independent from any specific technological solution, and in particular software application frameworks. Frameworks are invaluable for realistic development, but their continual evolution means that idiosyncratic knowledge required to use them has a short expectation of usefulness. Rather, this text focuses on general principles and techniques that underlie most frameworks.

## Module 0 - Preparation

How does one approach a software development project? Start hacking and hope for the best? Probably not. This would just be [inviting disaster](http://spectrum.ieee.org/static/the-staggering-impact-of-it-systems-gone-wrong). In this pseudo-module, I will present an overview of the important steps we need to take to prepare to develop quality software, from understanding the problem to mapping out a development process to choosing and setting up our tools to sketching an application.

[Module Notes](modules/Module-00.md)

## Module 1 - Encapsulation

One of the major motivation for good design is to keep control of the complexity of a system. An idea that is paramount to simplifying the design of software is encapsulation. Ideally, classes serve to support functionality, but also to isolate distinct computations. This module will cover the most important concepts and techniques necessary to design well-encapsulated classes.

[Module Notes](modules/Module-01.md)

## Module 2 - Types and Polymorphism

One of the main mechanisms at our disposal for designing object-oriented applications is *polymorphism*, which in the case of Java and similar languages is heavily tied to the notion of a type system. In this module I will do a brief review of the foundations of polymorphism, introduce the idea of interface programming, and present common low-level design problems that are easily solved with polymorphism.

[Module Notes](modules/Module-02.md)

## Module 3 - Object State

The most difficult thing to reason about when looking at a program is state changes. What operations can have a side-effect, on which path can data flow, what impacts what? Is this module, I will clarify what object state is and how we can manage to keep control over its state in a principled way so we don't let the genie out of the bottle every time we instantiate an object.

[Module Notes](modules/Module-03.md)

## Module 4 - Unit Testing

How can we have confidence that our code is working properly? Every time we write or change a line of code, we could be introducing a lethal bug. *Unit testing* is a practice wherein we automatically execute our code to check that it does what we think it should. With unit testing, we can build a possibly large collection of tests that can quickly be run, for instance every time we change the code, to make sure we didn't break anything that used to work. In this module, I will introduce mechanisms that facilitate unit testing (reflection and type annotations) and provide you with basic techniques for designing unit tests and evaluating their quality.

[Module Notes](modules/Module-04.md)

## Module 5 - Composition

Large programs are typically assembled from smaller parts. In object-oriented programming this is done through two main mechanism: *composition* and *inheritance*. Composition simply means that one object holds a reference to another object and delegates some tasks to it. Although this sounds simple enough, unprincipled composition can lead to a terrible mess of spaghetti code. In this module I will give a quick refresher on the mechanism of polymorphism and how it can be used to elegantly compose objects together by following some well-known design patterns. Note that the second way of assembling systems is through inheritance, which is more complex and will be covered in Module 7.

[Module Notes](modules/Module-05.md)

## Module 6 - Inversion of Control

The idea of inversion of control is one of the most powerful intellectual tools in a software designer tool-box. It allows us to build incredibly sophisticated applications while keeping the overall design complexity down to a manageable level. The Observer pattern is extremely common in software development, and it's realized by most GUI toolkits on most software development platforms, from desktop to web to mobile applications. This module is dedicated to the principle of inversion of control (IoC) and its realization in the Observer pattern, also called the Model-View Controller (MVC) pattern.

[Module Notes](modules/Module-06.md)

## Module 7 - Inheritance

*Inheritance* is a programming language-supported mechanism that allows us to assemble state and computation from different classes into a single object. It is a powerful feature that offers a natural solution to many design problems related to code extensibility and dynamic configuration. At the same time, it is a complex mechanism that can all too easily be misused. In this module, I will offer a review of inheritance and present the major design rules and patterns involving it.

[Module Notes](modules/Module-07.md)

## Module 8 - Design Patterns

This module will explore design solutions that incorporate design patterns an inheritance and introduce the Visitor design pattern.

[Module Notes](modules/Module-08.md)

## Module 9 - Concurrency

*Concurrent programming* is a paradigm that allows developers to write code that can execute in parallel (on multi-core systems) or with the illusion of parallelism (on single-core ones). Concurrent programming is very, very challenging and is ideally only used in support of well-defined and well-understood design problems, such as performing background operations or displaying animations. In fact, many typical concurrent programming problems already have a framework-based solution that hides the use of concurrency primitives. In this module, I will present the foundations of object-oriented concurrent programming and a few examples of the use of concurrency in practice.

[Module Notes](modules/Module-09.md)

## Module 10 - Serialization

Sometimes, the data in a running program needs to be transferred out of the program, for example to be stored in a file or transmitted over a network. In this module, I will cover the main techniques for serializing object graphs using a variety of frameworks including Java's binary serialization and JavaBeans frameworks and JSON serialization APIs. This module will also feature an introduction to the agile development practice called refactoring.

[Module Notes](modules/Module-10.md)

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a>

Unless otherwise noted, the content of this repository is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>. 

Copyright Martin P. Robillard 2017
