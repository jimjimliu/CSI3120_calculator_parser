# CSI3120 calculator parser

## How to run

Download the given “partial folder”. Substitute the four altered source files into the folder. First locate the source file folder in the terminal. There is a .sh file called build_partial.sh, run it in the terminal. It would create a executable file in the source folder, and some other necessary files if successfully complied. Then run the executable; we can test the calculator with our input there.


Implement a calculator language using Lex and yacc (or Flex and Bison). The calculator language must:
• handle integers only;
• have a unspecified number of variable that varies according to the user input;
• implement addition (+), subtraction (-), multiplication (*), division (/), and modulus
operators (%);
• Have all operators aforementioned left-associative;
• implement the non-associative unary minus (-) operator;
• implement assignment statements using the operator (=);
• multiplication and division have higher precedence than addition and subtraction;
• allow the of use parentheses to override operator precedence;
You may implement a delimiter of statements, for instance ‘;’ (as in Java, C, or C++); Implement an interpreter that executes statements during the parsing process.

You must implement a printing instruction that shows the value of a given variable or expression. Your interpreter may terminate upon a syntax error.
Hints:
1) Remember that Lex and Flex implement the lexical units recognizer using regular expressions; 2) Yacc and Bison are PDA based parsers, so you don’t have to worry about left recursion;
3) Yacc and Bison cannot handle ambiguous grammars, you must specify if operators are left or right recursive;
4) Implement the first draft of your calculator with only addition and subtraction operators;
5) Implement all operators with the simple symbol table present in the example provided with the assignment description; After you implementing all the operator try to implement a more complete version of a symbol table, try using hashes or maps;
6) If you implement the inner workings of your calculator in C use gcc to compile it, if you use C++ use g++
Deliverables:
1) Lex file, with tokens and regular expressions used to recognize tokens (.l);
2) Yacc file, with BNF (.y);
3) Working calculator interpreter;
4) PDF with BNF, tokens descriptions (with regular expressions and examples), instructions of how to compile and use your interpreter.
*The example provided has a fixed symbol table size, the variables identifiers are simple lowercase characters ‘a’, ‘b’...
**You are allowed (maybe encouraged) to use the wonders of C++ to create a calculator with unspecified number or variables.
***You may also use Python-Lex-Yacc to create your parser interpreter.
