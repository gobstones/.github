# **Gobstones**

## About
This organization is devoted to the **Gobstones** project, and it is aimed to programmers. 
If you want to contribute, there are _**a lot**_ of ways to do it, not only programming.
If you want to know more about **Gobstones**, how to contribute to it, or the related material, refer to the [home page](http://gobstones.org).
Also, at the end of these document we add a [brief explanation of what constitutes **Gobstones**](#about-gobstones) for the casual reader and completion.

Ths _Github_ organization was created to home the repositories implementing to the programming environment of the project, **GobstonesWeb**.
There are repositories with different purposes: some deal with organization issues, and others are related to different versions of the environment.
More about repositories in the sections [GobstonesWeb2 repositories](#gobstonesweb2-repositories) and [Other repositories](#other-repositories).

### How to get help
If you want to join the organization or get help on something related to it, please join the [**Gobstones Community**](https://bit.ly/ComunidadGobstones) at _Discord_, and follow the rules of the organization to receive a proper role.

### Programming environments
The environment currently deployed (in its 3 modes: [**GobstonesJr**](https://gobstones.github.io/gobstones-jr/), [**GobstonesSr**](https://gobstones.github.io/gobstones-sr/) and [**GobstonesTeacher**](https://gobstones.github.io/gobstones-teacher/)) was started on 2015 and developed mostly by a single developer (with some contributions from other programmers), without too much planning in advance regarding architecture, modifiability, or long term growing. The technologies for development weren't chosen with a plan in mind, and soon became obsolete (for example, it uses _Polymer_ for component integration, a preliminary version of _Blockly_ that was not published as a release, and other currently deprecated). For that reason, making any change or improvement is a complex and very error prone task.

The development team decided to start a new version of the environment, **GobstonesWeb2**, providing first a similar functionality to the current one, but with a more solid architecture, modern technologies, and a workflow warranteeing modifiability and future growth.
While the repositories for the current environment are still present, they will not be further mantained. 
Eventually they will be properly separated.

## **Architecture of GobstonesWeb2**
Understanding **GobstonesWeb2** requires to know a non-trivial amount of information.
There are a lot of components to understand, a lot of technologies used that you should be aware of, and, if you want to contribute, also a series of guidelines to understand the workflow and the rules your source code must comply.

To know more about the guidelines to contribute, consult [Gobstones-Guidelines](https://github.com/gobstones/gobstones-guidelines).

### **GobstonesWeb2 repositories**
The architecture of **GobstonesWeb2** combines several modules providing different functionalities.
For each module, there will be a repository in the organization.
The guidelines ask for all repositories  to share a basic configuration structure, and in order to ensure it, there is a special module, in repository [gobstones-scripts](https://github.com/gobstones/gobstones-scripts),that all repositories of **GobstonesWeb2** must depend on. 
In this way, when the team decide to change something on the common configuration, all repositories can be easily updated.

The architecture of **GobstonesWeb2** is established by the dependencies between the modules provided by the different repositories belonging to the project, as presented in the following diagram:

![GobstonesWeb2 Architecture Diagram](https://github.com/gobstones/.github/blob/new-readme/Diagrama%20de%20Componentes%20del%20Proyecto%20Gobstones.svg)

<details>
<summary>List of repositories of <b>GobstonesWeb2</b></summary>
<p>

The complete list of repositories to be used on **GobstonesWeb2** (either planned or under development).
* [`gobstones-admin-dashboard`](https://github.com/gobstones/gobstones/gobstones-admin-dashboard), a dashboard for the Gobstones server, 
* [`gobstones-assertions`](https://github.com/gobstones/gobstones/gobstones-assertions), a static and semantic code analyzer for Gobstones langauge, 
* [`gobstones-blocks`](https://github.com/gobstones/gobstones-blocks), a framework agnostic Gobstones Blockly component, 
* [`gobstones-blocks-react`](https://github.com/gobstones/gobstones/gobstones-blocks-react), the REACT layer over gobstones-blocks,
* [`gobstones-board`](https://github.com/gobstones/gobstones/gobstones-board), a representation for Gobstones boards,
* [`gobstones-board-react`](https://github.com/gobstones/gobstones/gobstones-board-react), the REACT layer over the gobstones-board,
* [`gobstones-code-editor`](https://github.com/gobstones/gobstones/gobstones-code-editor), a code editor to use with Gobstones,
* [`gobstones-core`](https://github.com/gobstones/gobstones-core), a set of utility tools used through all GobstonesWeb2 repositories,
* [`gobstones-ide`](https://github.com/gobstones/gobstones-ide), the IDE component, with the actual enviornment, 
* [`gobstones-gbb-parser`](https://github.com/gobstones/gobstones-gbb-parser), a parser/printer for GBB (Gobstones Board) file format,
* [`gobstones-guidelines`](https://github.com/gobstones/gobstones/gobstones-guidelines), fundamental documentation to contribute to GobstonesWeb2,
* [`gobstones-lang`](https://github.com/gobstones/gobstones/gobstones-lang), a compiler for Gobstones language,
* [`gobstones-lang-intl`](https://github.com/gobstones/gobstones-lang-intl), translation for Gobstones language built-ins and keywords, 
* [`gobstones-lint`](https://github.com/gobstones/gobstones/gobstones-lint), a linter for Gobstones language,
* [`gobstones-markdown-view`](https://github.com/gobstones/gobstones/gobstones-markdown-view), a markdown viewer for Gobstones,
* [`gobstones-parser`](https://github.com/gobstones/gobstones-parser), a parser for Gobstones language v3.12,
* [`gobstones-refactors`](https://github.com/gobstones/gobstones/gobstones-refactors), a refactoring tool for Gobstones language
* [`gobstones-scripts`](https://github.com/gobstones/gobstones-scripts), common configuration for all GobstonesWeb2 repositories
* [`gobstones-server`](https://github.com/gobstones/gobstones/gobstones-server), the Gobstones server,
* [`gobstones-test`](https://github.com/gobstones/gobstones/gobstones-test), a unit testing framework for Gobstones language,
* [`gobstones-typechecker`](https://github.com/gobstones/gobstones/gobstones-typechecker), a typechecker for Gobstones language.

Not in the diagram:
* [`gobstones-api-docs`](https://github.com/gobstones/gobstones/gobstones-api-docs), an API Docs web page for GobstonesWeb (does not appear in the diagram),
* [`template-gobstones-typescript-library`](https://github.com/gobstones/gobstones/template-gobstones-typescript-library), a template project to create new typescript languages for the Gobstones platform (does not appear in the diagram).
<details>
<summary>To determine</summary>
<p>

These repositories have to be determined about their purpose.
* `gobstones-board-react-refactor` - Refactoring of the gobstones-board-react proyect (lmattera)
* `gobstones-classroom-server` - API for the administration of Gobstones courses and tracking of students' progress (JuanEscalada)
* `gobstones-backoffice` - Gobstones Backoffice Client (JuanEscalada)
</p>
</details>
</p>
</details>


## **Other repositories**
There are 3 repositories related with the organization:
* [`.github`](https://github.com/gobstones/.github), the home for the Gobstones organization, containing this README,
* [`gobstones.github.io`](https://github.com/gobstones/gobstones.github.io), the current website for Gobstones in Github, and
* [`gobstones-website`](https://github.com/gobstones/gobstones-website), the website for Gobstones community.

Other repositories that do not belong to `Organization` or to `GobstonesWeb2` correspond to components related with old versiones of the enviornment (current environment and **PyGobstones**) or aborted experiments.

<details>
<summary>List of repositories of the current environment</summary>
<p>

* [`ace-builds`](http://github.com/gobstones/ace-builds), packaged version of Ace code editor, 
* [`course-creator`](http://github.com/gobstones/course-creator), a tool to create courses for GobstonesWeb, 
* [`editor-beta` ](http://github.com/gobstones/editor-beta), an editor to process Gobstones dinamically, 
* [`gobstones-activity-server`](http://github.com/gobstones/gobstones-activity-server), a buffer for activities from Github to GobstonesWeb,
* [`gobstones-cli`](http://github.com/gobstones/gobstones-cli), the CLI for gobstones-intepreter, 
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
