
# Project Name: AetherC

## Description
AetherC is a comprehensive C compiler project aimed at providing a robust toolchain for compiling C code into optimized NASM assembly language. The project includes modules for tokenization, parsing, semantic analysis, code generation, semantic validation, and preprocessing.

## Features
- Lexer for tokenization of source code.
- Parser for constructing Abstract Syntax Tree (AST).
- Resolver for semantic analysis and symbol table generation.
- Code generator for NASM assembly output.
- Semantic validator for ensuring code correctness.
- Preprocessor for handling directives and macros.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AetherC.git
   cd AetherC
   ```

2. Build the project:
   ```bash
   make build
   ```

3. Run tests (optional):
   ```bash
   make test
   ```

## Usage
1. Compile C code:
   ```bash
   ./aetherc source_file.c -o output_file.asm
   ```

2. Run generated assembly code (example using NASM and GCC):
   ```bash
   nasm -f elf64 -o output_file.o output_file.asm
   gcc -o executable_name output_file.o
   ./executable_name
   ```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature_branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature_branch`).
6. Create a new Pull Request.


## Acknowledgements
- [NASM](https://www.nasm.us) for the NASM assembler.
