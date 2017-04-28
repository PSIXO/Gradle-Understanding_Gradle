# Core concepts

Main unit of gradle logic is called a **project**  
Project can have children which are called **modules** (words project and module can be used interchangeability and both represent instances of Project objects on which gradle process will work)  
Both project and modules contain some logic to execute which is regarded as **tasks**  
Each task can consist of multiple **actions**  
Both project and modules have their own **build scripts** in which logic for the build is declared

Each call to gradle binary is regarded as a **build**
Builds consist of **3 phases**:

*	**Initialization** During the initialization phase, Gradle determines which projects are part in the build.
*	**Configuration** During this phase the project objects are configured. The build scripts of all projects which are part of the build are executed.
*	**Execution** Gradle determines the subset of the tasks, created and configured during the configuration phase, to be executed. Which tasks will be executed depends on the names passed to gradle via command line and current directory.

Also important thing to note about gradle and especially its **execution** stage is that tasks defined can be linked to each other in **directed acyclic graph** and graph connections determine which **tasks** are dependent on which other tasks.

Additionally some more options to create **connections** between tasks are available which do not introduce task dependencies but only ordering. These are **must run after**, **should run after** and **finalizedBy**




