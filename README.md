# CSC530-project1
Sun, 24 Jan 2021 You shall develop, test, and deliver a program which will print the contents of a 
“regular file” to the terminal (stdout). 
 
This basic file-printer, or “dump”, program will open the file specified by the 
user when launching the program from the command line and shall read every byte in 
the file, printing both the value of each byte as well as it is printable (human-
readable) character (characters, digits, symbols). 
 
The output has three fields in each record (line of output)  
1.  The address of the first byte of this record 
2.  The file content by bytes 
3.  ASCII encoded characters of the bytes printed in this record* 
 
Defaults: 
1.  The bytes from the file will be printed using hex, in octets (2 bytes/4 hex 
chars), each octet spaced by a single space char, 16 octets per record 
2.  When binary option is selected, the bytes from the file will be printed one 
byte at a time using bits (binary chars 1 or 0), 8 bytes per record 
 
* Note – in the 3rd column, print only “human readable ASCII chars.  For the non-
printable characters, your program shall print a ‘.’ character (a dot/period 
character, i.e. hex value 2E).  Your executable file shall be named “dump”. 
 
Example hex output (file fragment): 
0003540: 0504 0675 6e73 6967 6e65 6420 6368 6172  ...unsigned char 
0003550: 0008 0107 0000 0131 0675 6e73 6967 6e65  .......1.unsigne 
 
Example binary output (file fragment): 
0003540: 00000101 00000100 00000110 01110101 01101110 01110011 01101001 01100111 ...unsig 
0003548: 01101110 01100101 01100100 00100000 01100011 01101000 01100001 01110010 ned char 
 
Create directory ~/a1 by hand on edoras in your class account.  Then create C/C++ 
source file(s), a Makefile, and a README file, put them into ~/a1. 
 
Note, your dump program will only open regular file type (binary or text/ASCII 
content), you are not required to handle other file types or errors encountered if 
the user attempted to run your dump program on other file types (dir, special, 
link, pipe). 
 
Suggestion – become familiar with the xxd program on edoras. 
 
Running your dump program:  You will build your program such that the dump program 
will be launched as follows from the shell’s command line: 
   edoras% dump <filename> 
   edoras% dump –b <filename> 
 
the first example will cause your dump program to print the contents of the file 
specified by <filename> in hex format.  The second example will cause your dump 
program to print the file specified by <filename> in binary format.  
 
ADDITIONAL REQUIREMENTS: 
README file - you shall create a README file; consult the instructions for README 
file content on the course in Canvas.  Also, your source files SHALL CONTAIN 
sufficient comments for making the source easy to read. Points will be taken off 
for poorly (or non) commented source or inadequate README file documentation. 
 
Compiler and Make – You shall use a C/C++ (gcc/g++ on edoras) compiler to compile 
your project. You will also use the make program to direct the compilation of your 
project for this project, this will require you to create a file named Makefile.  
If you do not have experience with make, consult the example Reference Module in 
the course on Canvas.  The name of the executable needs to be to ‘dump’. 
 
Project teams.  This project is individual work.  You may discuss ideas and 
challenges with friends and other students but all work must be your own (do not 
share files in whole or any parts). 
 
TURNING IN YOUR WORK: 
When you are ready to turn this project in, ensure that all of your files are ready 
for testing on edoras (leave them there). 
 
Additionally, turn-in your project using Canvas’ Assignment turnin feature. I need 
two files uploaded into Canvas Assignment #1: a tarball/zipfile (containing the 
source code file(s), README file, any additional files you may have created), and, 
a README (text) file  
