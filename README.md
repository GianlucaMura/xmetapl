XMETAProgrammingLanguage (v1.0)<br/>is a general metalanguage which, through its AST semantics, allows its code to be executed in the browser and convertible into other languages.
<br/><br>SEMANTIC ELEMENTS(AST):<br/>
- prog{type:"prog", prog:[ AST..]}The Program
- proto{type:"proto", vars:[ NAME..], body: AST }Function
- call{type:"call", func:AST,args:[ AST..]}Call
- var{type:var, value: NAME }Variable
- num{type:"num", value:NUMBER}Type Number
- str{type:"str", value:STRING}Type string
- bool{type:"bool", value:true or false}Type Boolean
- if{type:"if", cond:AST, then:AST, else:AST}IF Condition
- assign{type: "assign", operator:"=", left:AST, right:AST}Assignement
- binary{type: "binary", operator:OPERATOR, left:AST, right:AST} + - * / % && || < > <= => == !=

AST Description(Abstract Semantic Tree)<br/>
In computer science, an abstract syntax tree (AST),is a tree representation of the abstract syntactic structure of the source code written in a formal language.They are data structures widely used in compilers to represent the structure of program code. It often serves as an intermediate representation of the program through several stages that the compiler requires.

XMETAPL<br/>
The Program is a sequence of instructions. Xmpl uses expressions instead of declarations. Expressions return a value and each can be used in place of another expression. ';' separate expressions into a sequence of statements. '{' create sequences as well as expressions '}' Functions are introduced by the proto keyword. After proto a list of variables separated by ',' between '(' and ')' is possible The body function is a single expression but can also be a sequence between '{' and '}' The last expression evaluated in a function, it returns its value to the calling function. For variables, a proto is used by declaring the variables as arguments. Variables have function scope.

PROGRAMMING ENVIRONMENT<br/>Primitive Functions<br/>
Primitive functions are a set of functions made available globally for utility.
- print() Write the output to the screen
- println() writes with carriage return

XMETAPL publication(10.2.23)<br/>
<br/>More improvement coming soon! Stay Tuned! Thanks!

<br/>Try it on http://www.artsmachine.org/v.php?p=xmetapl

Bibliography<br/>
- Wirth,Niklaus,"Algorithms+data structures=programs",Prentice-Hall,1976,USA
- Bazon,Mihai,https://lisperator.net
