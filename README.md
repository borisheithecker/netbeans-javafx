# netbeans-javafx


Demonstrates a possible solution to integrate JavaFX into a NetBeans RCP app build with jdk>11. 

It's a suite of three library wrapper modules providing the os-specifiy implementations of JavaFX. All three modules export an identical list of public packages, and all three of them are set to the same code-name-base. Only one module is referenced on the suite's module list, depending on property "javafx.os" in project.properties. 

To use this suite, set "javafx.os" in project.properties in accordance with you operating system and "clean build" the suite. Add the suite/cluster to you app. 

To build deployable zip files or installers for other operating systems, simple switch the variable and rebuild installers or the zip bundle. The zip bundle will be os-dependent. 
