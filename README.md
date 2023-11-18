# CS182-Project-1
This is the CS182 Project for UCR, we have chosen to do project 1. We will use JQF in the duration of the project.

# Section 1
In this section we are meant to download, compile, and run JQF from the source code.

Here is the instructions we followed:
Download JQF: git clone https://github.com/rohanpadhye/JQF
Compile JQF: After the clone command: mvn package
Download and Compile: git clone https://github.com/rohanpadhye/jqf && jqf/setup.sh

# Section 2
For this section, we are meant to install the test file and fuzz it through the JQF program. We are to use the javac command to install and compile the test file. 

Compile Command:  javac -cp .:$(/[path to]/jqf/scripts/classpath.sh) SimpleTest.java

The next part of section 2 was to fuzz the test file with the JQF program. We were meant to use the jqf-random command in order to fuzz the program.

Command we ran:  [path to]/jqf/bin/jqf-random -c .:$([path to]/jqf/scripts/classpath.sh) SimpleTest testSimpleTest 10

# Section 3
In this section, we are to modify the current source code for the JQF program and output the Event Ids with their respective branch arms. The compile command and the execution command are not altered in this session, except for the addition of -v before the SimpleTest portion of the execution command.

Command we ran:  [path to]/jqf/bin/jqf-random -c .:$([path to]/jqf/scripts/classpath.sh) -v SimpleTest testSimpleTest 10

# Section 4

In Section 4 of our project with JQF, our primary goal was to delve deeper into the intricacies of the Program Under Test (PUT) by employing controlled test inputs and enhancing the detail of output data for a more thorough analysis.


