Compiler Design Project: Switch Case Parser and TAC Generator

Description:
This project implements a parser for a simplified C-like language with switch-case statements and generates Three Address Code (TAC) as 
intermediate representation. The implementation includes:

A lexical analyzer (lexer) using Flex to tokenize input

A syntax analyzer (parser) using Bison to parse the grammar

TAC generation for switch-case control flow

Basic error handling with line number reporting

The program takes an input file containing switch-case statements and produces TAC output showing the control flow and temporary 
variables used in the computation.

Implementation Details:
The lexer (n.l) recognizes keywords, identifiers, numbers, and operators

The parser (n.y) handles the grammar rules and generates TAC

The output shows temporary variables (t1, t2, etc.) and labels (L1, L2, etc.) for control flow

Line numbers are tracked for error reporting

How to Build and Run:
Compile with: flex n.l && bison -d n.y && gcc lex.yy.c n.tab.c -o parser

Run with: ./parser input.txt output.txt

Author
Name: Dhruvi Patel
Roll Number: 22000402