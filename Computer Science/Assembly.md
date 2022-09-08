# Assembly language
#assembly

| Type | Example |
|------|----------|
| Directive | .file, .text, .global |
| Label | main: |
| Instructions | push, mov, ret |

.file "asm-0.c" - meta information that says which source code is the origin of the code
.text - states that the following is the program code/text
.globl main - says that main should be global in scope (visible to code in other files)

1. %register
2. $constant

**Directive** provides assembler with information.

**Labels** are used to refer to specific parts of the code.

