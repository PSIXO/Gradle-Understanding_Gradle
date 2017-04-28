# Or no installation

Gradle has a good solution to "Works on my machine problem"

*	Basic idea to solve this is to deploy build tool with the projects source
*	This is called the **gradle wrapper**
*	It is a group of scripts which can download and run specific gradle version
*	No installation of gradle is required to build a project
*	Gradle installation is required only for creating a wrapper and installed version can be any 2.4 version it does not need to be one used for wrapper

To create a wrapper run  
**_gradle wrapper --gradle-version 2.4_**
