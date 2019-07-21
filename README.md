Run tests

    GOPATH=`pwd` go test ./src/lexer
    GOPATH=`pwd` go test ./src/parser
    GOPATH=`pwd` go test ./src/evaluator

Run repl

    GOPATH=`pwd` go run ./src/main

Example repl output
    
    monkey-interpreter (master)$  GOPATH=`pwd` go run ./src/main.go 
    Hello mika! This is the Monkey programming language!
    Feel free to type in commands
    >> let add = fn(x,y) { x + y; };
    {Type:LET Literal:let}
    {Type:IDENT Literal:add}
    {Type:= Literal:=}
    {Type:FUNCTION Literal:fn}
    {Type:( Literal:(}
    {Type:IDENT Literal:x}
    {Type:, Literal:,}
    {Type:IDENT Literal:y}
    {Type:) Literal:)}
    {Type:{ Literal:{}
    {Type:IDENT Literal:x}
    {Type:+ Literal:+}
    {Type:IDENT Literal:y}
    {Type:; Literal:;}
    {Type:} Literal:}}
    {Type:; Literal:;}
    >> 

