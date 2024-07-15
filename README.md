**Huffman Coding Compression Project**

**Overview**

This project implements a Huffman Coding algorithm in C++ for text file compression. It includes the functionality to build a Huffman tree, generate Huffman codes, and compress text files using these codes.

**Features**

Huffman Tree Construction: Builds a Huffman tree based on the frequency of characters in the input file.
Huffman Code Generation: Generates Huffman codes for each character.
File Compression: Compresses the input file using the generated Huffman codes.
Bitwise Writing: Writes the compressed data bit by bit to the output file.
Compression Ratio Calculation: Calculates and displays the compression ratio achieved.

**Files**

**main.cpp** : Contains the implementation of the Huffman coding algorithm and file compression logic.
**Classes**
BitwiseWrite
The BitwiseWrite class handles bitwise writing to the output file.

Public Methods
BitwiseWrite(ostream & os): Constructor that initializes the output stream, buffer, and bit counter.
void flush(): Writes the buffer to the output file and clears it.
void writeBit(int i): Writes a bit to the buffer. Flushes the buffer if it is full or if i is -1.
MinHeapNode
The MinHeapNode struct represents a node in the Huffman tree.

**Members**
int data: The character data.
int freq: The frequency of the character.
**MinHeapNode left, right: Pointers to the left and right child nodes.
Functions
HuffmanCodes
The HuffmanCodes function builds the Huffman tree and generates Huffman codes.

**Parameters**

int data[]: Array of character ASCII values.
int freq[]: Array of character frequencies.
int size: The size of the data and frequency arrays.
printCodes
The printCodes function prints the Huffman codes by traversing the Huffman tree.

MinHeapNode root*: Pointer to the root of the Huffman tree.
string str: The Huffman code for the current node.
printTree
The printTree function prints the Huffman tree structure.

ostream & out: Output stream.
MinHeapNode root*: Pointer to the root of the Huffman tree.
int indent: Indentation level for tree structure visualization.

**Usage**

Running the Program
Compile the main.cpp file.
Run the executable and enter the name of the text file to compress.
The program will display the frequency table, Huffman codes, and Huffman tree.
The compressed file will be saved with a .cmp extension.
The program will display the compression ratio and a success message.
