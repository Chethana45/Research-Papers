# ✦ MiniForge
### Design and Implementation of a Custom Interpreted Programming Language

<p align="center">
  <img src="https://img.shields.io/badge/RESEARCH-PROGRAMMING_LANGUAGES-9B72CF?style=for-the-badge&labelColor=171923" />
  <img src="https://img.shields.io/badge/IMPLEMENTATION-C%2B%2B17-568CCB?style=for-the-badge&labelColor=171923" />
  <img src="https://img.shields.io/badge/DOMAIN-LANGUAGE_DESIGN-45A99A?style=for-the-badge&labelColor=171923" />
</p>

<p align="center">
  <i>Building a language from the ground up — from source code to execution.</i>
</p>

---

## ◈ About the Research

**MiniForge** is a custom interpreted programming language developed to explore programming language design, interpreter architecture, and runtime execution.

The project investigates how source code is transformed into executable behavior through a sequence of language-processing stages.

Implemented using C++17, MiniForge combines lexical analysis, recursive-descent parsing, abstract syntax trees, semantic analysis, and a tree-walk interpreter within a modular architecture.

The accompanying research paper explores the theoretical foundations, architectural design, implementation methodology, language features, testing observations, and possible future enhancements.

## ⌘ Research Objectives

- Design and implement a custom programming language.
- Develop a lexer for source-code tokenization.
- Implement recursive-descent parsing.
- Construct and process abstract syntax trees.
- Perform semantic analysis and validation.
- Develop a tree-walk interpreter.
- Implement runtime environments and lexical scoping.
- Support functions, recursion, arrays, and closures.
- Provide interactive and file-based execution.

## ⚙️ Technology Stack

| Component | Technology |
|---|---|
| Programming Language | C++17 |
| Build System | CMake |
| Parsing | Recursive-Descent Parser |
| Intermediate Representation | Abstract Syntax Tree |
| Execution Model | Tree-Walk Interpreter |
| Testing | GoogleTest, Custom Tests |
| Source File Extension | `.mf` |

## ◈ Core Language Features

- **Lexical Analysis** — Converts source characters into meaningful tokens.
- **Syntax Parsing** — Recognizes language structures using recursive-descent parsing.
- **Abstract Syntax Tree** — Represents program structure for further processing.
- **Semantic Analysis** — Performs supported semantic validation.
- **Variables and Expressions** — Supports fundamental programming constructs.
- **Control Flow** — Conditional statements and loops.
- **Functions and Recursion** — Enables reusable and recursive computations.
- **Arrays** — Supports indexed collections of values.
- **Lexical Scopes** — Organizes variable visibility.
- **Closures** — Preserves access to enclosing environments.
- **REPL** — Provides interactive program execution.
- **File Execution** — Runs programs through `.mf` source files.

## ▣ Implementation Architecture

The language follows a modular processing pipeline:

```text
SOURCE CODE
     |
     v
LEXICAL ANALYSIS
     |
     v
RECURSIVE-DESCENT PARSER
     |
     v
ABSTRACT SYNTAX TREE
     |
     v
SEMANTIC ANALYSIS
     |
     v
TREE-WALK INTERPRETER
     |
     v
RUNTIME ENVIRONMENT
     |
     v
PROGRAM EXECUTION
```

## ◇ Validation Summary

The reported development results include:

| Validation | Result |
|---|---|
| C++17 Compilation | Successful |
| Automated Test Suite | 5 Tests Passed |
| Factorial Evaluation | Expected result: 120 |
| Closure Evaluation | Expected output: 1 2 |
| REPL | Implemented |
| `.mf` File Execution | Implemented |

*Results are based on the project's development records and do not represent independent benchmarking or exhaustive language validation.*

## 📄 Research Paper

The accompanying IEEE-style research paper covers:

1. Introduction and research objectives.
2. Background and related work.
3. Programming language architecture.
4. Lexer and parser implementation.
5. Abstract syntax tree design.
6. Semantic analysis and runtime environments.
7. Language features and execution methodology.
8. Testing and evaluation.
9. Limitations and future enhancements.
10. Technical references.

## ◈ Limitations and Future Work

Potential future enhancements include:

- Bytecode generation and virtual-machine execution.
- Improved runtime memory management.
- Extended type-system capabilities.
- Expanded standard library.
- Advanced debugging and diagnostics.
- Performance benchmarking.
- More extensive automated testing.

A bytecode virtual machine is a future direction, not part of the current tree-walk interpreter.

## 👩‍💻 Researcher

**Chethana Sri**

Department of Computer Technology  
Madras Institute of Technology, Anna University  
Chennai, India

<p align="center">
  <a href="https://github.com/Chethana45">
    <img src="https://img.shields.io/badge/GitHub-Chethana45-171923?style=for-the-badge&logo=github" />
  </a>
</p>

---

<p align="center">
  <b>MINIFORGE</b>
  <br/>
  <i>From language design to executable ideas.</i>
  <br/><br/>
  ✦ Design. Parse. Interpret. Create. ✦
</p>
