cmake_minimum_required(VERSION 3.20)
project(minilang)

set(CMAKE_CXX_STANDARD 23)

add_executable(minilang
        src/main.cpp
        src/lexer/lexer.cpp
        src/lexer/lexer.h
        src/lexer/token.cpp
        src/lexer/token.h
        src/parser/parser.cpp
        src/parser/parser.h
        src/parser/ast.cpp
        src/parser/ast.h
        src/visitor/visitor.h
        src/visitor/xml_visitor.cpp
        src/visitor/xml_visitor.h
        src/visitor/semantic_analysis.cpp
        src/visitor/semantic_analysis.h
        src/visitor/interpreter.cpp
        src/visitor/interpreter.h
        src/table/table.h)