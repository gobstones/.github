# **Gobstones**

## **About**
This organization is devoted to the **Gobstones** project, and it is aimed to programmers. 
If you want to contribute, there are _**a lot**_ of ways to do it, not only programming.
If you want to know more about **Gobstones**, how to contribute to it, or the related material, refer to the [home page](http://gobstones.org).
Also, at the end of these document we add a [brief explanation of what constitutes **Gobstones**](#about-gobstones) for the casual reader and completion.

The _Github_ Organization was created to home the repositories implementing to the programming environment of the project, **GobstonesWeb**.
There are repositories with different purposes: some deal with organization issues, and others are related to different versions of the environment.
More about repositories in the sections [GobstonesWeb2 repositories](#gobstonesweb2-repositories) and [Other repositories](#other-repositories).

### How to get help
If you want to join the organization or get help on something related to it, please join the [**Gobstones** Community](https://bit.ly/ComunidadGobstones) at _Discord_, and follow the rules of the server to receive a proper role.

### Programming environments
The environment currently deployed (in its 3 modes: [**GobstonesJr**](https://gobstones.github.io/gobstones-jr/), [**GobstonesSr**](https://gobstones.github.io/gobstones-sr/) and [**GobstonesTeacher**](https://gobstones.github.io/gobstones-teacher/)) was started on 2015 and developed mostly by a single developer (with some contributions from other programmers), without too much planning in advance regarding architecture, modifiability, or long term growing. The technologies for development weren't chosen with a plan in mind, and soon became obsolete (for example, it uses _Polymer_ for component integration, a preliminary version of _Blockly_ that was not published as a release, and other currently deprecated). For that reason, making any change or improvement is a complex and very error prone task.

The development team decided to start a new version of the environment, **GobstonesWeb2**, providing first a similar functionality to the current one, but with a more solid architecture, modern technologies, and a workflow guaranteeing modifiability and future growth.
While the repositories for the current environment are still present, they will not be further maintained. 
Eventually they will be properly separated.

## **GobstonesWeb2 repositories**
Understanding **GobstonesWeb2** requires to know a non-trivial amount of information.
There are a lot of components to understand, a lot of technologies used that you should be aware of, and, if you want to contribute, also a series of guidelines to understand the workflow and the rules your source code must comply.

To know more about the guidelines to contribute, consult [Gobstones-Guidelines](https://github.com/gobstones/gobstones-guidelines).

### **Architecture of GobstonesWeb2**
The architecture of **GobstonesWeb2** combines several modules providing different functionalities.
For each module, there will be a repository in the organization.

We describe the list of repositories and their relationship [here](https://github.com/gobstones/gobstones-guidelines/blob/main/sections/gobstonesweb2-architecture.md).


## **Other repositories**
There are 3 repositories related with the organization:
* [`.github`](https://github.com/gobstones/.github), the home for the Gobstones organization, containing this README,
* [`gobstones.github.io`](https://github.com/gobstones/gobstones.github.io), the current website for Gobstones in Github, and
* [`gobstones-website`](https://github.com/gobstones/gobstones-website), the website for Gobstones community.

Other repositories that do not belong to `Organization` or to `GobstonesWeb2` correspond to components related with old versions of the environment (current environment and **PyGobstones**) or aborted experiments.

<details>
<summary>List of repositories of the current environment</summary>
<p>

* [`ace-builds`](http://github.com/gobstones/ace-builds), packaged version of Ace code editor, 
* [`course-creator`](http://github.com/gobstones/course-creator), a tool to create courses for GobstonesWeb, 
* [`editor-beta` ](http://github.com/gobstones/editor-beta), an editor to process Gobstones dynamically, 
* [`gobstones-activity-server`](http://github.com/gobstones/gobstones-activity-server), a buffer for activities from Github to GobstonesWeb,
* [`gobstones-cli`](http://github.com/gobstones/gobstones-cli), the CLI for gobstones-interpreter, 
* [`gobstones-code-runner`](http://github.com/gobstones/gobstones-code-runner), a tool to run Gobstones programs, 
* [`gobstones-issues`](http://github.com/gobstones/gobstones-issues), a storage to register users issues from GobstonesWeb, 
* [`gobstones-interpreter`](http://github.com/gobstones/gobstones-interpreter), the compiler for Gobstones language (wrongly named), 
* [`gobstones-jr`](http://github.com/gobstones/gobstones-jr), the GobstonesJr IDE, 
* [`gobstones-jr-staging`](http://github.com/gobstones/gobstones-jr-staging), alpha testing for new releases of GobstonesJr, 
* [`gobstones-minimal-server`](https://github.com/gobstones/gobstones/gobstones-minimal-server), a buffer between activities in Github and GobstonesWeb,
* [`gobstones-sr`](https://github.com/gobstones/gobstones-sr), the GobstonesSr IDE, 
* [`gobstones-sr-staging`](https://github.com/gobstones/gobstones-sr-staging), alpha testing for new releases of GobstonesSr, 
* [`gobstones-teacher`](https://github.com/gobstones/gobstones-teacher), the GobstonesTeacher IDE, 
* [`gobstones-teacher-staging`](https://github.com/gobstones/gobstones-teacher-staging), alpha testing for new releases of GobstonesTeacher, 
* [`gobstones-web`](https://github.com/gobstones/gobstones-web), the Gobstones Web IDE, 
* [`gobstones-web-desktop`](https://github.com/gobstones/gobstones-web-desktop), desktop version of GobstonesWeb, 
* [`gobstones-web-staging`](https://github.com/gobstones/gobstones-web-staging), alpha testing for new releases of GobstonesWeb, 
* [`gobstones-web-01-01-2018`](https://github.com/gobstones/gobstones-web-01-01-2018), snapshot of GobstonesWeb at 01-01-2018, 
* [`gs-board`](https://github.com/gobstones/gs-board), the Gobstones board for GobstonesWeb, 
* [`gs-board-render-test`](https://github.com/gobstones/gs-board-render-test), testing for Gobstones board render, 
* [`gs-element-blockly`](https://github.com/gobstones/gs-element-blockly), the Blockly element for GobstonesWeb, 
* [`gs-element-starter`](https://github.com/gobstones/gs-element-starter), starter template for a Gobstones Web polymer element, 
* [`gs-weblang-core`](https://github.com/gobstones/gs-weblang-core), (DEPRECATED) use gobstones-interpreter, 
* [`keymaster`](https://github.com/gobstones/keymaster), a simple micro-library for defining and dispatching keyboard shortcuts with no dependencies.
</p>
</details>

## **About Gobstones**
**Gobstones** is a project started at National University of Quilmes in 2008 by Pablo E. --Fidel-- Martínez López and Eduardo Bonelli. 
The motivation for the project was the seek for am innovative didactics proposal in order to teach programming with very precise goals, to people with no prior experience on programming.

In order to meet that goal, they designed a programming language that capture the main ideas of the proposed didactics, and started to use it in their lectures.
Soon it was obvious that a programming environment integrating both the language and the didactics was needed.
So, **Gobstones** involves three elements:
* a _didactics proposal_,
* a _programming language_, designed to capture the idea of that didactics, and 
* a _programming environment_, integrating both the didactics and the language.

Those 3 elements grew up along time, usually with rich interrelationships between them
The name **Gobstones** was initially used for the programming language, but as the language was conceived with a particular didactics in mind, the same name was used also for that didactics proposal.
The programming environment always was named with a different name (usually containing also the name **Gobstones** in it), depending on the different implementations and the technologies used for that.
The current version used web technologies, and for that reason it is called **GobstonesWeb**. 
However, most people use the name **Gobstones** _also_ to refer to the environment.
