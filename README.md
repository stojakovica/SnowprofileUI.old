Copyright (c) 2012 Aleksandar Stojakovic
 
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
 
The Software shall be used for Good, not Evil.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

*) I recommend to work with Eclipse (http://www.eclipse.org/) and import the 
project into Eclipse


1) Building with gradle
-------------------------------------------------------------------------------

First install Gradle (http://www.gradle.org/). Make sure you have configured the
PATH for gradle and test gradle with the command "gradle --version". For
downloading all dependencies and librarys you have to build the gradle-build-file
"build.gradle". For building in eclipse you have to build with the command
"gradle cleanEclipse eclipse".


2) Sources
-------------------------------------------------------------------------------

The source-files of the Java-Project is an Eclipse-created Project and is located
in the "Snowprofile"-folder. For starting just compile the ServerMain.java file in the
package "at.ac.dbisinformatik.snowprofile.app" after finishing step 1).
When compiled you can start the Web Application in your Browser by typing:
"http://127.0.0.1:8080/lwd/"

3) Export as runable Project
-------------------------------------------------------------------------------

When everything works well you can export the project as a runable binary-File.
Just use the command "gradle distZip" and it will create a folder "distribution" where
the whole Project is exported as a Zip-File. Unzip the File on your Server and start
the Snowprofile-File in the folder "bin" (Snowprofile.bat for Windows-Server) with screen
and your Web Application is avaible on your Server.