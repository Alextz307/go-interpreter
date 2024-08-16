# Writing an Interpreter in Go

This repository contains the source code from the book *Writing an Interpreter in Go* by Thorsten Ball. The book walks through the development of an interpreter for a simple programming language called Monkey, written in Go.

## Table of Contents

1. [Overview](#overview)
2. [Project Structure](#project-structure)
3. [Getting Started](#getting-started)
4. [Usage](#usage)
5. [Tests](#tests)
6. [Contributing](#contributing)
7. [License](#license)

## Overview

*Writing an Interpreter in Go* is a hands-on guide to creating an interpreter from scratch. The book is designed for programmers who are curious about how interpreters work and want to deepen their understanding by building one step by step.

In this repository, you'll find all the source code as it's developed throughout the book. The Monkey programming language, which the interpreter is designed to execute, is a small, C-like language with features such as:

- Variable bindings
- Functions and closures
- Data structures like arrays and hashes
- Built-in functions

## Project Structure

The repository is organized into the following directories:

- `lexer/`: Contains the lexical analyzer, which breaks the input text into tokens.
- `parser/`: Includes the code for the parser, which builds an Abstract Syntax Tree (AST) from the tokens.
- `ast/`: Defines the data structures for the AST.
- `evaluator/`: Implements the interpreter logic, evaluating the AST.
- `object/`: Represents the various data types in the Monkey language.
- `repl/`: Contains the code for the Read-Eval-Print Loop (REPL) of the interpreter.
- `main.go`: The entry point of the interpreter, which launches the REPL.

## Getting Started

### Prerequisites

To run the code in this repository, you'll need:

- [Go](https://golang.org/doc/install) version 1.16 or higher.

### Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/Alextz307/interpreter-in-go.git
    cd interpreter-in-go
    ```

2. Build the interpreter:

    ```sh
    go build -o monkey
    ```

3. Run the REPL:

    ```sh
    ./monkey
    ```

## Usage

After launching the interpreter, you can start typing Monkey code directly into the REPL. Here are a few examples:

```monkey
let x = 10;
let y = 20;
x + y;
```

The interpreter will evaluate the expressions and print the results.

## Tests

The repository includes unit tests for various components of the interpreter. To run the tests, use the following command:

```sh
go test ./...
```

This will execute all tests in the repository and provide feedback on the code's correctness.

## Contributing

Contributions are welcome! If you find bugs or have suggestions for improvements, please open an issue or submit a pull request.

Before submitting a pull request, please make sure that:

1. Your code passes all the tests.
2. Your code follows the style guidelines.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
