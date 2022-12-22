# **Gobstones**

## Introduction
This organization is devoted to the **Gobstones** project, and it is aimed to programmers. 
If you want to contribute, there are _**a lot**_ of ways to do it, not only programming.
If you want to know more about **Gobstones**, how to contribute to it, or the related material, refer to the [home page](http://gobstones.org).
Also, at the end of these document we add a [brief explanation of what constitutes **Gobstones**](#about-gobstones) for the casual reader and completion.

Ths _Github_ organization was created to home the repositories implementing to the programming environment of the project, **GobstonesWeb**.

The environment currently deployed (in its 3 modes: [**GobstonesJr**](https://gobstones.github.io/gobstones-jr/), [**GobstonesSr**](https://gobstones.github.io/gobstones-sr/) and [**GobstonesTeacher**](https://gobstones.github.io/gobstones-teacher/)) was started on 2015 and developed mostly by a single developer (with some contributions from other programmers), without too much planning in advance regarding architecture, modifiability, or long term growing. The technologies for development weren't chosen with a plan in mind, and soon became obsolete (for example, it uses _Polymer_ for component integration, a preliminary version of _Blockly_ that was not published as a release, and other currently deprecated). For that reason, making any change or improvement is a complex and very error prone task.

The development team decided to start a new version of the environment, **GobstonesWeb2**, providing first a similar functionality to the current one, but with a more solid architecture, modern technologies, and a workflow warranteeing modifiability and future growth.
While the repositories for the current environment are still present, they will not be further mantained. 
Eventually they will be properly separated.

## **Architecture and workflow for GobstonesWeb2**
Understanding **GobstonesWeb2** requires to know a non-trivial amount of information.
There are a lot of components to understand, a lot of technologies used that you should be aware of, and, if you want to contribute, also a series of guidelines to understand the workflow and the rules your source code must comply.

To know more about the guidelines to contribute, consult [Gobstones-Guidelines](https://github.com/gobstones/gobstones-guidelines).

More about the architecture will be explained here (_HELP NEEDED_).

## About Gobstones
**Gobstones** is a project started at Universidad Nacional de Quilmes in 2008 by Pablo E. --Fidel-- Martínez López and Eduardo Bonelli. 
The motivation for the project was the seek for am innovative didactics proposal in order to teach programming with very precise goals, to people with no prior experience on programming.

In order to meet that goal, they designed a programming language that capture the main ideas of the proposed didactics, and started to use it in their lectures.
Soon it was obvious that a programming environment integrating both the language and the didactics was needed.
So, **Gobstones** involves three elements:
* a _didactics proposal_,
* a _programming language_, designed to capture the idea of that didactics, and 
* a _programming environment_, integrating both the didactics and the language.

Those 3 elements grew up along time, usually with rich interrelationships between them
The name **Gobstones** was initially used for the programming language, but as the language was concieved with a particular didactics in mind, the same name was used also for that didactics proposal.
The programming environment always was named with a different name (usually containing also the name **Gobstones** in it), depending on the different implementations and the technologies used for that.
The current version used web technologies, and for that reason it is called **GobstonesWeb**. 
However, most people use the name **Gobstones** _also_ to refer to the environment.
