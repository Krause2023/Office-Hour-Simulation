# *Professor Office Hour Simulation*

## Description
**_Simulation of Professor's Office Hour Schedule_** <br/>
The simulation program takes data provided in an input file and creates a schedule for a professor's office hours. The information provided in the input includes the following information: </br>

**Information regarding the professor** </br>
• The name of the professor </br>
• The professor's number of availalbe minutes reserved for office hours on Monday </br>
• The professor's number of availalbe minutes reserved for office hours on Tuesday </br>
• The professor's number of availalbe minutes reserved for office hours on Wednesday </br>
• The professor's number of availalbe minutes reserved for office hours on Thursday </br>
• The professor's number of availalbe minutes reserved for office hours on Friday

**Information regarding the students** </br>
• The number of students </br>
• The name of each student </br>
• The type of visit that the student is going to offic hours for (**Q** for question, **D** for demo, **A** for advising) </br>
• The visit length for the student (in minutes) </br>
• The day(s) the student is available to visit the professor in office hours

If you want to see an example of output for the simulation, see the `picture of the output with a FIFO queue implemented` below this description. The simulation uses different algorithms to create an output that shows what students the professor will see on a given day, how the professor is helping the student(s) on a given day, the number of students that visited the professor in his office hours on a given day, the number of students who waited to visit the professor in his office hours on a given day, the number of minutes spent with students in a given day, and the number of minutes students waited to attend office hours with the professor in a given day. At the end of the printed output, summary statistics are given to show the total number of students that the professor met with, the total amount of time taken in office hours, and the total amount of time that students waited to visit the professor in office hours for the week. </br>
This program was written using the C programming languge. The simulation program was made as a final project for one of my Computer Science classes (CS 270) at the University of Wisconsin - La Crosse.

###### Example of Program Output on Terminal using a FIFO Queue
<img width="569" alt="exampleoutput" src="https://user-images.githubusercontent.com/57727121/132105157-df2e45a4-fd5b-48c5-b379-4426da2b3737.png">
<p>&nbsp;</p>

**Resources for Project:**
- C (Programming language)
- Atom (Text editor)
- Terminal / Command Line

# Running / Viewing the Project
## Command Line
1. First, make sure that you have your terminal open. Information about your terminal can be found here: <br/>
   -Mac: https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac <br/>
   -Windows: https://docs.microsoft.com/en-us/windows/terminal/
2. Next, check if you have the C compiler already installed in your system. If you are using the UNIX / Linux operating systems in your terminal, then you likely have a C compiler called GCC in your system. To determine if you already have GCC installed in your system, type `cc --version` or `gcc --version` in your terminal. Information regarding the version of your C Compiler will show on the terminal after you enter a "--version" command. The C programming language is already built into your system (regardless of what computer / operating system you have). For more information on C and C compilers, click the link below. <br/>
   -C Compiler Information: https://www.w3schools.in/c-tutorial/install/
3. On this repository page, go to the "Code" button and click the "Download Zip" option.
4. Go to your "Downloads" section on your computer and place the zip file in a folder/location other than "Downloads".
5. Double click on the zip file to open or "unzip" it so you can access the file contents.
6. In your opened terminal, navigate to the location where you opened the downloaded zip file and make sure you are inside of the "Office-Hour-Simulation-master" folder. (If you are unsure of command line commands, see the resources provided bellow.) <br/>
   -Linux and Max: http://mally.stanford.edu/~sr/computing/basic-unix.html <br/>
   -Windows: https://blogs.umass.edu/Techbytes/2014/11/14/file-navigation-with-windows-command-prompt/
7. Inside of the "Office-Hour-Simulation-master" folder on your terminal, navigate into the "office-simulation" folder.
8. Inside of the "office-simulation" folder, type the following command: `make simulator-final`. We are using the C compiler along with a Makefile that was provided in this project to compile the code, which is why we type "make" in the command. As a result, an executable file is created called "simulator".
9. After typing the command above, type this command: `./simulator -f infile1.txt`. Here we are running the compiled version of the program (the executable file), which we named "simulation". The argument flag listed after the executable file tells the program what kind of algorithm to run in the program (A FIFO queue). We also pass a text file, included in this project, into the program to be read and analyzed.
10. After running the command in the previous step, output should be printed out on your terminal window. Information about other command arguments you can use is provided below. </br>
    -To indicate that FIFO is being used, a "-f" flag is used as the first command-line argument. <br/>
    -To indicate that advising appointments are being prioritized, a "-a" flag is used as the first command-line argument. <br/>
    -To indicate that project demos are prioritized, a "-d" flag is used as the first command-line argument. <br/>
    -To indicate that project questions are prioritized, a "-q" flag is used as the first command-line argument. <br/>
    -Example input file are provided in the forms of infile1.txt, infile2.txt, and infile3.txt. Each of these files can be passed through the program when it is run as the second command line argument.
11. Try using the other argument flags, "-a", "-d", and "-q", when you run the office hour simulation program. Also, try running the program using the other files, infile2.txt and infile3.txt. To view the text files, you can open them using a text editor. You can also type the `cat` command and then the name of the text file to view the contents of the text file on your terminal (Example: `cat infile1.txt` lets you see the file contents of infile1.txt).
12. To learn more about Makefiles, and priority queues, visit the following links below. </br>
      -Makefiles: https://makefiletutorial.com/ </br>
      -Priority queues: https://www.geeksforgeeks.org/queue-data-structure/
13. NOTE: To recompile your program, if neccessary, first type `make clean` to clear the compiled files. Then type `make simulator-final` to recompile everything.

<p>&nbsp;</p>

**_@Author: Andrew Krause_** <br/>
*LinkedIn:* https://www.linkedin.com/in/andrew-krause-b6aa21179/ <br/>
*Portfolio:* https://andrewkrause.dev/ <br/>
*Instagram:* https://www.instagram.com/aek.krause/ <br/>
*Facebook:* https://www.facebook.com/andrew.krause.35325

