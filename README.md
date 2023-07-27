# CDSS
This repository contains all the C, Lex, and Yacc programs that I have executed for my CDSS Course
How to Run
Ensure that you have a C compiler installed on your system.

gcc --version
It should look something like this GCC Version

If you don't have a C compiler installed, you can download one from here or using your package manager.

Examples:

Ubuntu -
sudo apt install gcc
Arch Linux -
sudo pacman -S gcc
macOS -
brew install gcc
Additionaly, if you are using Windows, follow the steps specified here.

Clone the repository using the following command:

gh repo clone rexgraystone/cdss
or

git clone https://github.com/rexgraystone/cdss.git
Change the directory to the cloned repository:

cd cdss
For Lex programs:

Compile the Lex program using the following command:

lex <filename>.l
Example:

lex 1a_CharCount.l
Compile the generated C file using the following command:

gcc lex.yy.c -ll -o <Output File Name>
Run the program using the following command:

./<Output File Name>
For YACC programs:

Compile the Lex program using the following command:

lex <filename>.l
Example:

lex 4_EvalExpressions.l
Compile the YACC program using the following command:

yacc -d <filename>.y
Example:

yacc -d 4_EvalExpressions.y
Compile the generated C file using the following command:

gcc lex.yy.c y.tab.c -ll -o <Output File Name>
