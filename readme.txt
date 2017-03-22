December 10, 2001


LAWRENCEVILLE PRESS LIBRARIES

The Lawrenceville Press libraries needed by most of the programs presented in
A Guide to Programming in C++ are stored in the LVP folder on this diskette. In
order for programs to have access to these library files, create a folder named
LVP in the INCLUDE folder of the compiler's root directory. For example, for
Turbo C++ version 4.5, the directory structure would appear like
C:\TCWIN45\INCLUDE\LVP. For Microsoft Visual C++ version 5,the directory
structure would appear like C:\PROGRAM FILES\DEVSTUDIO\VC\INCLUDE\LVP. For
Microsoft Visual C++ version 6,the directory structure would appear like
C:\PROGRAM FILES\MICROSOFT VISUAL STUDIO\VC98\INCLUDE\LVP. Next,
copy the files in the LVP folder on this diskette to the LVP folder created in
your compiler's INCLUDE folder.

IMPORTANT*********************************************************************
The lvp libraries are functionally equivalent to the AP libraries. Therefore,
the lvp libraries are updated when the AP libraries are updated. To insure that
you are using the most up-to-date libraries, please periodically download the
library files from the Lawrenceville Press web site by going to
http://www.lvp.com, clicking the Download button, clicking the Data Files links,
scrolling to the bottom of the download files page, and then clicking the 
appropriate link.


BORLAND TURBO C++\BORLAND C++ USERS

The programs in the PROGS_TC folder on this diskette correspond to the programs
presented in the text. The programs have been given descriptive names according
to their opening comments.

The programs in Chapter Six that use the college library require the
colleges.txt file. This file is stored in the TEXT folder on this diskette.

Many of the programs in Chapter Nine require text (.txt or .dat) files. These
files are stored in the TEXT folder on this diskette.


MICROSOFT VISUAL C++ 5.0\6.0 USERS

To create a project workspace and run an existing program, such as a program on
this diskette, use the following instructions:
1. Start Microsoft Visual C++.
2. From the File menu, select the New command.
3. Create a new Win32 console application project (Version 6.0 users create an
   empty Win32 console application project).
4. From the Project menu, select the Add To Project command and then the Files
   command.
5. Select the appropriate C++ file.

The programs in Chapter Six that use the college library require the college.txt
file. This file is stored in the TEXT folder on this diskette.

Many of the programs in Chapter Nine require text (.txt or .dat) files. These
files are stored in the TEXT folder on this diskette.

A set of programs corresponding to the programs presented in the text have been modified to 
work with Microsoft Visual C++. The programs are stored in the PROGS_MC folder and have 
been given descriptive names based on their opening comments. Microsoft Visual C++ does not 
support many of the conio functions. Programs corresponding to Section 4.21 are not included 
with the PROGS_MC programs. It is recommended that Microsoft Visual C++ users skip Section 
4.21 of the text. Changes made to the programs in this set include the following:

doodle.cpp
Because gotoxy() and clreol() are not supported by Microsoft Visual C++, the doodle 
program is not included in the PROGS_MC folder.

sturecs.cpp
Because getche() is not supported by Microsoft Visual C++, the line of code in 
main() that reads char Choice = getche(); in the text has been changed to the lines
char Choice;  cin >> Choice; in the program on diskette.

case3.cpp
The iostream library included with MSV requires a call to unsetf() in order to
change alignment of output, as stated in Appendix B of A Guide to Programming
in C++. Therefore, the line cout.unsetf(ios::left); was added prior to every
line that reads cout.setf(ios::right);. Three of these lines were added to
case3.cpp.

case7.cpp
Because clrscr() is not supported by Microsoft Visual C++, it was commented 
out in main().

case8.cpp
The iostream library included with MSV requires a call to unsetf() in order to
change alignment of output, as stated in Appendix B of A Guide to Programming
in C++. Therefore, the line cout.unsetf(ios::left); was added prior to every
line that reads cout.setf(ios::right);. Two of these lines were added to
case8.cpp: one in DisplayCandidateRow() and one in DisplayAll().

case9.cpp
Because getche() is not supported by Microsoft Visual C++, the two lines of code that
read Choice = getche();  cout << endl; were changed to cin >> Choice;
cin.ignore(80, '\n'); The cin.ignore() function is needed because getline() will
read the end of line character that is still in the stream. Refer to Chapter
Three (p. 3-11). This change was made in ChangeBook() and main().

case10.cpp
Because getche() is not supported by Microsoft Visual C++, the two lines of code 
above the case statement that read Choice = getche();  cout << endl; were changed to 
cin >> Choice; cin.ignore(80, '\n'); The cin.ignore() function is needed because
getline() will read the end of line character that is still in the stream. Refer
to Chapter Three (p. 3-11.)


CODEWARRIOR LEARNING EDITION VERSION 2 USERS

The Lawrenceville Press library files for CodeWarrior Learning Edition, v2 for the 
PC are stored in the lvpcw folder on master diskette #1. These files are needed by most 
of the programs presented in A Guide to Programming in C++. In order for programs to 
access these library files, they must be copied to the compiler’s appropriate INCLUDE 
folder. In this case, the destination should be very similar to:
C:\Program Files\Metrowerks\CW Learning Edition 2\MSL\MSL_C++\MSL_COMMOM\INCLUDE

Creating a C++ Project in CodeWarrior Learning Edition, v2

To create a project and run an existing program, such as a program provided on the 
master diskettes, use the following instructions:

1. Start CodeWarrior.

2. Select File -> New. The New dialog box is displayed.
a. Select Win32 C++ Stationery.
b. Type a descriptive name in the Project Name box.
c. Select Set to change the project location, if necessary.
d. Select OK. The New Project dialog box is displayed.
e. Click + beside Win32 Console App, if necessary.
f. Click C++ Console App.
g. Select OK. The project manager window is displayed.

3. In the project manager window, click + beside the Source folder. The Source folder contents 
are displayed. Note the hello.cpp file. This file is a temporary, test file that will be 
deleted later.

4. Click the Source folder to select it, if necessary.

5. Select Project -> Add Files. The Select files to add dialog box is displayed.
a. Use the Look in list and the contents box below it to select an existing C++ program.
b. Select Add. The Add Files dialog box is displayed.
c. Select OK. The file has been added to the Source folder and the Project Messages window 
appears.

6. In the project manager window, right-click hello.cpp and select Delete. A warning dialog box 
is displayed.
a. Select OK. hello.cpp is removed from the project.

7. If needed, double-click the added source file name to display it in a text editor window and 
then make modifications.
a. Select File -> Save. The modified file is saved.

8. Select Project -> Run. The application is compiled and run. If errors or warnings are 
encountered,a window is displayed with the appropriate messages.

To create a new file to be added to a project, perform steps 1 through 4 above and then do the 
following before skipping ahead to step 8 above:

Select File -> New. A dialog box is displayed.
a. Select the File tab.
b. In the File list, click Text File.
c. In the File name box, type a descriptive name being sure to include the .cpp extension.
d. The Location box should already display the appropriate project folder. However, if needed, 
use Set to select the appropriate project.
e. Select the Add to project check box.
f. The Project list should already have the appropriate project selected.
g. Select the C++ Console App Debug and the C++ Console App Release check boxes.
h. Select OK. A window is displayed for the new text file.
i. Type the application code.
j. Select File -> Save.

Some programs require additional data files (TXT and DAT files), including programs in 
Chapter 6, Chapter 9, and Chapter 12. For these programs, perform steps 1 through 7 above 
and then do the following before continuing with step 8 above:

Select Edit -> C++ Console App Debug Settings. A dialog box is displayed.
a. In the Target Settings Panels, select Runtime Settings from the Target list.
b. In the Working Directory box, type the path of the data file.
c. Select OK.

Chapter 11 presents graphics programming. For the programs associated with this chapter, the 
file project stationery is Win32 GUI App (Step 2e above) and Win 32 C++ App (Step 2f above). 
The temporary test file that should be deleted is called HelloWin32.cpp (Steps 3 and 6 above).

Library and Program Changes

A set of programs corresponding to the programs presented in the text have been modified to 
work with CodeWarrior Learning Edition version 2, for the PC. The programs have been given 
descriptive names based on their opening comments. Changes made to the programs in this set 
include the following:

#include
Because the library files are copied directly to the Include folder and not placed in a 
subfolder named lvp, the lvp directory path in any #include statements needs to be deleted.

using namespace std;
The line using namespace std; has been added after the #include statements in each program 
and library file.

string.h
#include <lvp\string.h> has been changed to #include <lvpstring.h>.

vector.h
#include <lvp\vector.h> has been changed to #include <lvpvector.h>.

random.h
#include <lvp\random.h> has been changed to #include <lvprandom.h>.

stack.h
#include <lvp\stack.h> has been changed to #include <lvpstack.h>.

queue.h
#include <lvp\queue.h> has been changed to #include <lvpqueue.h>.

bool.h
#include <lvp\bool.h> has been commented out because CodeWarrior has a built-in bool type.

conio.h
#include <conio.h> has been commented out because CodeWarrior does not support these 
library functions.

stopwatc.h
CodeWarrior does not support the functions used in stopwatc.h.

CodeWarrior does not support the conio library functions discussed in Section 4.12. 
Therefore, doodle.cpp is not provided as part of the program set. Reviews and exercises 
related to this section should be skipped.

string.h
Because CodeWarrior has a string library, the lvp library files string.h and string.cpp have 
been renamed lvpstring.h and lvpstring.cpp. Programs that use the string.h library need to be 
modified so that the include statement reads #include <lvpstring.h> and String definitions 
read lvpstring. The easiest way to do this is to use the Find command from the Search menu.

vector.h
Because CodeWarrior has a vector library, the lvp library files vector.h and vector.cpp have 
been renamed lvpvector.h and lvpvector.cpp. Programs that use the vector.h library need to 
be modified so that the include statement reads #include <lvpvector.h> and vector definitions 
read lvpvector. The easiest way to do this is to use the Find command from the Search menu.

random.h
Because CodeWarrior has a random library, the lvp library file random.h has been renamed 
lvprandom.h. Programs that use the random.h library need to be modified so that the 
include statement reads #include <lvprandom.h> and random(...) statements read lvprandom(...). 
The easiest way to do this is to use the Find command from the Search menu.

stack.h
Because CodeWarrior has a stack library, the lvp library files stack.h and stack.cpp have been 
renamed lvpstack.h and lvpstack.cpp. Programs that use the stack.h library need to be modified 
so that the include statement reads #include <lvpstack.h> and stack definitions read lvpstack. 
The easiest way to do this is to use the Find command from the Search menu.

queue.h
Because CodeWarrior has a queue library, the lvp library files queue.h and queue.cpp have been 
renamed lvpqueue.h and lvpqueue.cpp. Programs that use the queue.h library need to be modified 
so that the include statement reads #include <lvpqueue.h> and queue definitions read lvpqueue. 
The easiest way to do this is to use the Find command from the Search menu.

bool.h
Because CodeWarrior has a built-in bool type, the lvp bool.h and bool.cpp library files are 
not required and are therefore not included with the library file set. Programs that use bool 
need to be modified so that the #include <lvp\bool.h> statement is commented out.

sturecs.cpp
Because CodeWarrior does not support conio.h, the line of code in main() that reads char 
Choice = getche(); in the text has been changed to the lines char Choice; cin >> Choice;

case3.cpp
The iostream library included with CodeWarrior requires a call to unsetf() in order to 
change alignment of output. Therefore, the line cout.unsetf(ios::left); was added prior 
to every line that reads cout.setf(ios::right); and the line cout.unsetf(ios::right); was 
added prior to every line that reads cout.setf(ios::left). Six of these lines were added 
to case3.cpp.

case6.cpp
Because of a change in a library file, the line of code in main() that reads 
EnrollmentList.Clear(); has been changed to EnrollmentList.ClearData(); The iostream library 
included with CodeWarrior requires a call to unsetf() in order to change alignment of output. 
Therefore, the line cout.unsetf(ios::left); was added prior to every line that reads 
cout.setf(ios::right); and the line cout.unsetf(ios::right); was added prior to every line 
that reads cout.setf(ios::left). Two of these lines were added to case6.cpp.

case7.cpp
Because CodeWarrior does not support conio.h, clrscr() was commented out in main().

case8.cpp
The iostream library included with CodeWarrior requires a call to unsetf() in order to change 
alignment of output. Therefore, the line cout.unsetf(ios::left); was added prior to every line 
that reads cout.setf(ios::right); and the line cout.unsetf(ios::right); was added prior to 
every line that reads cout.setf(ios::left). Two of these lines were added to case8.cpp.

case9.cpp
Because CodeWarrior does not support conio.h, the two lines of code that read Choice = getche(); 
cout << endl; needed to be changed to cin >> Choice; cin.ignore(80, ‘\n’); The cin.ignore() 
function is needed because getline() will read the end of line character that is still in the 
stream. Refer to Chapter Three (p. 3-11). This change was made in ChangeBook() and main().

The line of code in main() that reads:
fstream BookFile("BookData.txt", ios::in | ios::out);
has been changed to the following lines of code:

fstream CheckFileExist;
CheckFileExist.open("BookData.txt", ios::in | ios::out); 
if (CheckFileExist.fail()) { 
ofstream CreateFile("BookData.txt"); 
CreateFile.close(); 
} 

CheckFileExist.close(); 
fstream BookFile; 
BookFile.open("BookData.txt", ios::in | ios::out); 

case10.cpp
Because CodeWarrior does not support conio.h, the lines of code above the case statement that 
read Choice = getche(); cout << endl; needed to be changed to cin >> Choice; cin.ignore(80, ‘\n’); 
The cin.ignore() function is needed because getline() will read the end of line character that is 
still in the stream. Refer to Chapter Three (p. 3-11.) The line of code in the beginning of 
main() that reads fstream BankData; needed to be deleted. The line of code in the beginning of 
main() that reads BankData.open("Bankdata.dat",ios::in); has been changed so that it reads 
ifstream BankData("bankdata.dat");. Change the line of code in the end of main() that reads 
BankData.open("bankdata.dat",ios::out); so that it reads ofstream BankDataOut("bankdata.dat"); 
and BankData in the following lines of code has been changed to BankDataOut:

BankData << NumAccounts << endl;
Bank[AcctNum].Store(BankData);
BankData.close();

utility.h
Because CodeWarrior does not support conio.h, the #include <conio.h> statement has been commented 
out. Because CodeWarrior does not support getch(), the lines of code in Pause() needed to be 
changed to:

char choice;
cout << "Press a key and then Enter to continue";
cin >> choice; //Pause for the user to press a key and then Enter
cout << endl;

hanoir.cpp
Because CodeWarrior does not support getch(), the line of code in Hanoi() that reads getch() 
needed to be changed to Pause().

When using files and steams:

1. ifstream does not create a file if it does not exist

2. ofstream does create a file if it does not exist

3. fstream does not create a file if it does not exist and open() needs to be used to check if 
the file exists

4. CodeWarrior does not support nocreate

5. to find the number of characters in a file, use the following instead of the code in 
section 9.14:

streampos Position;
MyFile.seekg(0,ios::end);
Position = MyFile.tellg();
cout << Position.offset();

readfile.cpp
Because CodeWarrior does not support nocreate, the line of code in main() that reads ifstream 
InFile("ask-not.txt", ios::nocreate); has been changed to ifstream InFile("ask-not.txt");

readscor.cpp
Because CodeWarrior does not support nocreate, the line of code in main() that reads ifstream 
InFile("scores.dat", ios::nocreate); has been changed to ifstream InFile("scores.dat");

readchar.cpp
Because CodeWarrior does not support nocreate, the line of code in main() that reads ifstream 
InFile("quick.txt", ios::nocreate); has been changed to ifstream InFile("quick.txt");

filestat.cpp
Because CodeWarrior does not support nocreate, the line of code in main() that reads 
InFile.open(FileName.c_str(),ios::nocreate); has been changed to InFile.open(FileName.c_str());. 
The line of code in main() that reads ifstream InFile; has been moved to before the line of 
code that reads InFile.open(FileName.c_str());.

rwfile.cpp
The line of code in main() that reads fstream MyFile("composer.txt", ios::in | ios::out); 
has been changed to: 
fstream MyFile;
MyFile.open("composer.txt",ios::in | ios::out);

stopwatc.h
The functions required in stopwatc.h are not supported by CodeWarrior and therefore stopwatc.h 
is not included with the library file set. Programs that use this library need to be modified 
so that the #include <lvp\stopwatc.h> statement is commented out.




TECHNICAL SUPPORT

Lawrenceville Press Technical Support
cpphelp@lvp.com
(561) 265-4664  fax 24 hours
(561) 265-0033  phone 9 a.m. to 5 p.m. EST



