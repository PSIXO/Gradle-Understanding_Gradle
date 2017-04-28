# Important files

*	**build.gradle** file used to define the build logic for our build, when using multi-module builds each module can have its own build.gradle
*	**settings.gradle** used to define modules in a multi module-build, typically we use the keyword **include** 'folder name' to include a module is specific folder
*	**gradle.properties** use this file to define additional parameters to use in gradle build, these can also be passed in from command line using **_-Poption=value_** syntax

All files listed above should be added to version control and shared along with the project. If we would like to have some local setting (like for example setting android sdk path) we should use
*	**local.properties** meaning and sintax of this file is the same as above gradle.properties but by common convention this file is not added to version control

