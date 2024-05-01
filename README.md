# -Booth-s-Signed-Multiplication-Algorithm

Using C programming language implement the Booth’s Signed Multiplication Algorithm. In this algorithm,
you will use the input file input.txt. In your algorithm you are going to perform n number of
multiplications. For each multiplication, first read the number of bits, and in the next line, read two binary
numbers with that number of bits.
Each multiplication will have the following output:

## Multiply 1001 and 0011
Product Q-1 M -M Log
0000 0011 0 1001 0111 Populate Data
0111 0011 0 1001 0111 A = A - M
0011 1001 1 1001 0111 Shift
0001 1100 1 1001 0111 Shift
1010 1100 1 1001 0111 A = A + M
1101 0110 0 1001 0111 Shift
1110 1011 0 1001 0111 Shift

1001 * 0011 = 11101011

-7 * 3 = - 21

### The input.txt file will be as follows:
n // count of multiplications
bits // number of bits
n1 n2 // binary signed numbers n1 and n2
bits // number of bits
n1 n2 // binary signed numbers n1 and n2
bits // number of bits
n1 n2 // binary signed numbers n1 and n2
...
bits // number of bits
n1 n2 // binary signed numbers n1 and n2

### Please use the following function signatures:
- int binaryToDecimal(char *binary)
- char *decimalToBinary(int input)
- char *take2sComplement(char *in)
- boothMultiply(char* n1, char* n2)
// This function will read one multiplication operation inputs: read number of bits, will allocate memory
// according to number of bits, and will read n1 and n2.
- void readMultiplicationOperation(file* pInfile, char** pN1, char** pN2)
