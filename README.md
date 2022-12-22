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

## **Architecture and workflow for GobstonesWeb2**
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

The complete list of repositories to be used on **GobstonesWeb2** (either planned or on development).
* `gobstones-admin-dashboard`
* `gobstones-assertions`
* `gobstones-blocks`
* `gobstones-blocks-react`
* `gobstones-board`
* `gobstones-board-react`
* `gobstones-code-editor`
* `gobstones-core`
* `gobstones-ide`
* `gobstones-gbb-parser`
* `gobstones-guidelines`
* `gobstones-lang`
* `gobstones-lang-intl`
* `gobstones-lint`
* `gobstones-markdown-view`
* `gobstones-parser`
* `gobstones-refactors`
* `gobstones-scripts`
* `gobstones-server`
* `gobstones-test`
* `gobstones-typechecker`

* `gobstones-minimal-server` -- ¿Este está en GobstonesWeb2? No aparece en el diagrama
* `gobstones-api-docs` -- ¿Este está en GobstonesWeb2? No aparece en el diagrama
* `template-gobstones-typescript-library` -- ¿Este está en GobstonesWeb2? No aparece en el diagrama

Reconstruir la historia de estos
* `gobstones-board-react-refactor` - Refactoring of the gobstones-board-react proyect (lmattera)
* `gobstones-classroom-server` - API for the administration of Gobstones courses and tracking of students' progress (JuanEscalada)
* `gobstones-backoffice` - Gobstones Backoffice Client (JuanEscalada)

More about the architecture will be explained here (_HELP NEEDED_).

## Other repositories
There are 3 repositories related with the organization:
* `.github`, containing this README,
* `gobstones.github.io`, containing the current webpage, and
* `gobstones-website`, containing the new webpage.

Other repositories that do not belong to the Organization or to GobstonesWeb2 correspond to components related with old versiones of the enviornment (current GobstonesWeb and PyGobstones) or aborted experiments.

CHECK IF RELATED TO current environment
* `gobstones-web`
* `gobstones-web-staging`
* `gs-element-blockly`
* `gobstones-activity-server` - faloi
* `gs-board`
* `gobstones-web-desktop`
* `gobstones-cli`
* `gobstones-code-runner`
* `course-creator`
* `keymaster` - A simple micro-library for defining and dispatching keyboard shortcuts. It has no dependencies.
* `ace-builds`
* `gobstones-teacher-staging`
* `gobstones-teacher`
* `gobstones-jr-staging`
* `gobstones-jr`
* `gobstones-sr-staging`
* `gobstones-sr`
* `gobstones-issues`
* `gobstones-web-01-01-2018`
* `gs-board-render-test`
* `gs-weblang-core`
* `editor-beta` 
* `gs-element-starter`

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
