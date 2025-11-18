Hey Gökce

This is my interpretation of the filter CSV by age program.

## CSV Age Filter
----------------

This is a simple C program that reads a CSV file containing people and their ages, then filters out rows with an age greater than a specified maximum.

The program supports input from a file or `stdin`, and output to a file or `stdout`. It also handles malformed input gracefully and prints warnings or errors to `stderr`.


## Features:
---------------

- Read from file or standard input (`stdin`)
- Write to file or standard output (`stdout`)
- Validate and filter rows based on age
- Handle blank or malformed lines
- Suppress error messages in output file
- Simple and portable (ANSI C)


## Input Format:
----------------

CSV file where each line follows this structure:

- Name, Age

Example:

- Nuvi Våle, 18

- Aeral Körn
  
- Lumio Satō, 29


- Veski Ruañ, 12


The program handles the following errors (reported to stderr, not to the output file):

- Missing age after comma

- Blank lines

- Invalid or non-numeric age tokens

## Error Handling:
------------------

- Blank lines: "Error on line X: Blank line encountered."

- Missing age: "Error on line X: Age missing."

- Invalid age: "Error on line X: Age not recognized."

Errors are always printed to stderr and never to the output file.

---
