📘 Lexical Analyzer in C
📌 Overview

This project implements a Lexical Analyzer (Scanner) in C, which is the first phase of a compiler. The lexical analyzer reads source code from an input file and converts it into meaningful tokens such as keywords, identifiers, operators, numbers, and special symbols.

This project is developed as part of Compiler Design / System Programming Lab to understand the fundamentals of lexical analysis.

🎯 Objectives

To understand the working of the Lexical Analysis phase of a compiler.

To identify different types of tokens in source code.

To implement token recognition using C programming.

To demonstrate file handling and string manipulation in C.

🧠 What is a Lexical Analyzer?

A Lexical Analyzer is the first phase of a compiler.

It:

Reads the source program character by character.

Groups characters into meaningful sequences called tokens.

Removes whitespace and ignores irrelevant characters.

Passes tokens to the next compiler phase (Syntax Analyzer).

🏷️ Types of Tokens Identified

This program identifies:

✅ Keywords (int, float, if, while, return, etc.)

✅ Identifiers (variable names like x, sum)

✅ Operators (+, -, *, /, =)

✅ Numbers (integer constants)

✅ Special Symbols (;, ,, (), {})

🛠️ Technologies Used

C Programming Language

Standard Libraries:

stdio.h

ctype.h

string.h

File Handling in C

📂 Project Structure
Lexical-Analyzer/
│
├── lexical_analyzer.c
├── input.txt
└── README.md
▶️ How to Run the Program
Step 1: Clone the Repository
git clone https://github.com/your-username/lexical-analyzer.git
Step 2: Navigate to the Project Folder
cd lexical-analyzer
Step 3: Compile the Program
gcc lexical_analyzer.c -o lexer
Step 4: Run the Program
./lexer

Make sure the input.txt file is present in the same directory.

📄 Sample Input (input.txt)
int sum = 10;
float value = 20;
🖥️ Sample Output
int is a Keyword
sum is an Identifier
= is an Operator
10 is a Number
; is a Special Symbol
float is a Keyword
value is an Identifier
= is an Operator
20 is a Number
; is a Special Symbol
🔎 Working of the Program

The program opens the input file using fopen().

It reads characters using fgetc().

If a character is:

Alphabet → forms identifier/keyword

Digit → forms number

Operator symbol → prints operator

Special character → prints special symbol

Keywords are checked using strcmp() against a predefined list.

Tokens are printed with their type.

⚙️ Algorithm

Start

Open input file

Read character

If alphabet → form word → check keyword or identifier

If digit → form number

If operator → print operator

If special symbol → print symbol

Repeat until EOF

Stop

🚀 Features

Simple and beginner-friendly implementation

Uses file handling for input

Clear token classification

Easy to modify and extend

Suitable for academic submissions

📌 Limitations

Only supports basic keywords

Does not handle:

String literals

Floating point numbers (in advanced form)

Comments (//, /* */)

Multi-character operators (==, >=, etc.)

🔮 Future Enhancements

Add support for:

Comments removal

String literals

Floating-point constants

Multi-character operators

Improve error handling

Extend to full compiler front-end

Convert into GUI-based tool

Integrate into a mini compiler project

🎓 Academic Relevance

This project helps in understanding:

Compiler Design Concepts

Tokenization

Pattern Recognition

Basics of Language Processing

File Handling in C

👨‍💻 Author

Ritesh Yadav
B.Tech – Computer Science
Compiler Design Lab Project
