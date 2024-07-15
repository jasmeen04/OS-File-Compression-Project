# Huffman Coding Compression Project

This project implements a Huffman Coding algorithm in C++ for compressing text files. Huffman Coding is a popular algorithm used for lossless data compression by assigning shorter codes to more frequent characters and longer codes to less frequent characters.

# Features

**Huffman Tree Construction:** Constructs a Huffman tree based on the frequency of characters in the input text file.

**Huffman Code Generation:** Generates Huffman codes for each character based on the constructed Huffman tree.

**File Compression:** Compresses the input text file using the generated Huffman codes by replacing each character with its corresponding Huffman code.

**Bitwise Writing:** Utilizes bitwise operations to write the compressed data bit by bit into the output file, achieving efficient storage.

**Compression Ratio Calculation:** Calculates and displays the compression ratio achieved by comparing the sizes of the original and compressed files.

# Files

**main.cpp:** Contains the implementation of the Huffman coding algorithm, including the logic for tree construction, code generation, file compression, and ratio calculation.

# Classes

**BitwiseWrite**: Handles bitwise writing operations to the output file for efficient storage of compressed data.

# Functions and Methods

**HuffmanCodes:** Function to build the Huffman tree and generate Huffman codes based on character frequencies.

**printCodes:** Function to print the generated Huffman codes for each character after tree construction.

**printTree:** Function to visualize the structure of the Huffman tree, showing parent-child relationships and code assignments.

# Usage

**Running the Program:**

1) Compile main.cpp using a C++ compiler.
2) Execute the compiled executable and provide the name of the text file to compress.

**Program Execution Flow:**

1) The program reads the input text file and calculates the frequency of each character.
2) It constructs a Huffman tree using these frequencies and generates Huffman codes for each character.
3) After generating codes, it compresses the input file by replacing characters with their respective Huffman codes.
4) The compressed output is written to a file with a .cmp extension.
The program calculates and displays the compression ratio achieved.
Output:

During execution, the program displays the frequency table of characters, the generated Huffman codes, and the Huffman tree structure.
It concludes with a message indicating the success of the compression process and the achieved compression ratio.
This project demonstrates a fundamental application of Huffman Coding for text compression, providing insights into tree construction, code generation, and efficient data storage techniques using bitwise operations in C++.
