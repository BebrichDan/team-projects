# s21_matrix  

## Struct:
```
.
├── arithmetic
│   ├── s21_arithmetic.c
│   ├── s21_arithmetic.h
│   ├── s21_calc_complements.c
│   ├── s21_determinant.c
│   ├── s21_mult_matrix.c
│   ├── s21_mult_number.c
│   ├── s21_sub_matrix.c
│   └── s21_sum_matrix.c
├── coverage
│   ├── coverage.info
│   ├── html
│   │   ├── amber.png
│   │   ├── arithmetic
│   │   │   ├── index.html
│   │   │   ├── index-sort-f.html
│   │   │   ├── index-sort-l.html
│   │   │   ├── s21_arithmetic.c.func-c.html
│   │   │   ├── s21_arithmetic.c.func.html
│   │   │   ├── s21_arithmetic.c.gcov.html
│   │   │   ├── s21_calc_complements.c.func-c.html
│   │   │   ├── s21_calc_complements.c.func.html
│   │   │   ├── s21_calc_complements.c.gcov.html
│   │   │   ├── s21_determinant.c.func-c.html
│   │   │   ├── s21_determinant.c.func.html
│   │   │   ├── s21_determinant.c.gcov.html
│   │   │   ├── s21_mult_matrix.c.func-c.html
│   │   │   ├── s21_mult_matrix.c.func.html
│   │   │   ├── s21_mult_matrix.c.gcov.html
│   │   │   ├── s21_mult_number.c.func-c.html
│   │   │   ├── s21_mult_number.c.func.html
│   │   │   ├── s21_mult_number.c.gcov.html
│   │   │   ├── s21_sub_matrix.c.func-c.html
│   │   │   ├── s21_sub_matrix.c.func.html
│   │   │   ├── s21_sub_matrix.c.gcov.html
│   │   │   ├── s21_sum_matrix.c.func-c.html
│   │   │   ├── s21_sum_matrix.c.func.html
│   │   │   └── s21_sum_matrix.c.gcov.html
│   │   ├── cmd_line
│   │   ├── editor
│   │   │   ├── index.html
│   │   │   ├── index-sort-f.html
│   │   │   ├── index-sort-l.html
│   │   │   ├── s21_create_matrix.c.func-c.html
│   │   │   ├── s21_create_matrix.c.func.html
│   │   │   ├── s21_create_matrix.c.gcov.html
│   │   │   ├── s21_inverse_matrix.c.func-c.html
│   │   │   ├── s21_inverse_matrix.c.func.html
│   │   │   ├── s21_inverse_matrix.c.gcov.html
│   │   │   ├── s21_remove_matrix.c.func-c.html
│   │   │   ├── s21_remove_matrix.c.func.html
│   │   │   └── s21_remove_matrix.c.gcov.html
│   │   ├── emerald.png
│   │   ├── gcov.css
│   │   ├── glass.png
│   │   ├── index.html
│   │   ├── index-sort-f.html
│   │   ├── index-sort-l.html
│   │   ├── other
│   │   │   ├── index.html
│   │   │   ├── index-sort-f.html
│   │   │   ├── index-sort-l.html
│   │   │   ├── s21_eq_matrix.c.func-c.html
│   │   │   ├── s21_eq_matrix.c.func.html
│   │   │   ├── s21_eq_matrix.c.gcov.html
│   │   │   ├── s21_transpose.c.func-c.html
│   │   │   ├── s21_transpose.c.func.html
│   │   │   └── s21_transpose.c.gcov.html
│   │   ├── ruby.png
│   │   ├── snow.png
│   │   └── updown.png
│   └── *.info
├── editor
│   ├── s21_create_matrix.c
│   ├── s21_inverse_matrix.c
│   └── s21_remove_matrix.c
├── Makefile
├── other
│   ├── s21_eq_matrix.c
│   └── s21_transpose.c
├── s21_matrix.a
├── s21_matrix.h
├── test_main.c
└── tests
    ├── arithmetic_test
    │   ├── unit_test_calc_complements.c
    │   ├── unit_test_determinant.c
    │   ├── unit_test_mult_matrix.c
    │   ├── unit_test_mult_number.c
    │   ├── unit_test_sub_matrix.c
    │   └── unit_test_sum_matrix.c
    ├── editor_test
    │   ├── unit_test_create_matrix.c
    │   ├── unit_test_inverse_matrix.c
    │   └── unit_test_remove_matrix.c
    ├── other_test
    │   ├── unit_test_eq_matrix.c
    │   └── unit_test_transpose.c
    └── test
```

Implementation of the matrix.h library.   

💡 [Tap here](https://new.oprosso.net/p/4cb31ec3f47a4596bc758ea1861fb624) **to leave your feedback on the project**. It's anonymous and will help our team make your educational experience better. We recommend completing the survey immediately after the project.

## Contents  

1. [Chapter I](#chapter-i) \
   1.1. [Introduction](#introduction)
2. [Chapter II](#chapter-ii) \
   2.1. [Information](#information)
3. [Chapter III](#chapter-iii) \
   3.1. [Part 1](#part-1-implementation-of-the-matrixh-library-functions)


# Chapter I  

![matrix](misc/eng/images/matrixx.png)

Planet Earth, September 13, 2000.  

*"Our CEO has such a wonderful country house! It has everything you need to realise your ideas. A veranda overlooking a huge swimming pool on the lawn completes the picture of a keen and intelligent person."*

*"Yes, I agree, so glad we were invited here, this place is very energetic!"*  

*"Absolutely! So, for a few days now, the main id Software technical team have been discussing the new technology we want to introduce in our upcoming game Doom 3. What creates the most sense of reality in an image? Obviously it's a game of light and shadows, which now takes too long to calculate and puts a lot of pressure on the CPU. John is known for his technological and algorithmic ideas and tricks that have led to crazy breakthroughs in speed and code optimisation.* \
*What was I talking about... Our chief engineer and founder John Carmack presented a theoretical development that would allow you to cast shadows on a scene after it had gone through the entire graphics pipeline, using a depth and stencil buffer."* 

*"Oh wow, it gives me goosebumps, tell me more!"*

*"We didn't invite you to this party by chance, the whole team is working on a new way to create shadows in a scene, and John has specifically tasked your department with implementing a very fast and optimized library of all kinds of matrix transformations that will underpin all the mathematical logic of the algorithm: vectors and matrices, transpose and SRT transformations, and many other mathematical objects and operations used in computer graphics.* \
*FFor a proper and considered transition to the new method, we need a significant and impressive performance change, and you will be in charge of that!"*

*"My team and I are more than happy to help you, and are ready to get to work tomorrow!"*

*"Perfect! Who knows, maybe one day it will be enough just to cast the rays to create light and shadow... but for now, we're limited by the technology of our time and have to roll with the punches, so let's do it! And yes, don't you dare miss deadlines, he doesn't like that."*

## Introduction

In this project, you will implement your own library for processing numerical matrices in the C programming language. Matrices are one of the basic data structures in programming, used for example to represent table values, for computational tasks, and for neural networks. As part of this project, you will learn more about matrices and reinforce your knowledge of structured programming.


# Chapter II

## Information

### Historical Background

The first mentions of matrices (or as they were then called: "magic squares") were found in ancient China. \
They became famous in the middle of the 18th century thanks to the work of the famous mathematician Gabriel Cramer, who published his work "Introduction to the Analysis of Algebraic Curves", which described a fundamentally new algorithm for solving systems of linear equations. \
Soon after, the works of Carl Friedrich Gauss on the "classical" method of solving linear equations, the Cayley-Hamilton theorem, the works of Karl Weierstrass, Georg Frobenius, and other outstanding scientists were published. \
It was not until 1850 that James Joseph Sylvester introduced the term "matrix" in his work.

## Matrix

A matrix is a collection of numbers arranged in a fixed number of rows and columns.

Matrix A is a rectangular table of numbers arranged in m rows and n columns:

```
    1 2 3
A = 4 5 6
    7 8 9
```

```
     1  2  3  4
В =  5  6  7  8
     9 10 11 12
```

You can get the desired element with the help of indices, as follows
A[1,1] = 1, where the first index is the row number, the second is the column number.

Matrix A will have elements with the following indices:

```
    (1,1) (1,2) (1,3)
A = (2,1) (2,2) (2,3)
    (3,1) (3,2) (3,3)
```

The order of a matrix is the number of its rows or columns. \
The main diagonal of a square matrix is the diagonal from the upper left to the lower right corner. \
A rectangular matrix (B) is a matrix with the number of rows not equal to the number of columns. \
A square matrix (A) is a matrix with the number of rows equal to the number of columns.

A column matrix is a matrix with only one column:

```
    (1,1)
A = (2,1)
    (n,1)
```

A row matrix is a matrix that has only one row:

```
A = (1,1) (1,2) (1,m)
```

Tip: A column matrix and a row matrix are also often called vectors.

A diagonal matrix is a square matrix in which all elements outside the main diagonal are zero. \
An identity matrix is a diagonal matrix with all diagonal elements equal to one:

```
    1 0 0
A = 0 1 0
    0 0 1
```

A triangular matrix is a square matrix with all elements on one side of the main diagonal equal to zero.

```
    1 2 3
A = 0 4 5
    0 0 6
```

### Matrix structure in C language:

```c
typedef struct matrix_struct {
    double** matrix;
    int rows;
    int columns;
} matrix_t;
```
## Matrix operations

All operations (except matrix comparison) should return the resulting code:
- 0 - OK
- 1 - Error, incorrect matrix
- 2 - Calculation error (mismatched matrix sizes; matrix for which calculations cannot be performed, etc.)

### Creating matrices (create_matrix)

```c
int s21_create_matrix(int rows, int columns, matrix_t *result);
```

### Cleaning of matrices (remove_matrix)

```c
void s21_remove_matrix(matrix_t *A);
```

### Matrix comparison (eq_matrix)

```c
#define SUCCESS 1
#define FAILURE 0

int s21_eq_matrix(matrix_t *A, matrix_t *B);
```

The matrices A, B are equal |A = B| if they have the same dimensions and the corresponding elements are identical, thus for all i and j: A(i,j) = B(i,j)

The comparison must be up to and including 7 decimal places.

### Adding (sum_matrix) and subtracting matrices (sub_matrix)

```c
int s21_sum_matrix(matrix_t *A, matrix_t *B, matrix_t *result);
int s21_sub_matrix(matrix_t *A, matrix_t *B, matrix_t *result);
```

The sum of two matrices A = m × n and B = m × n of the same size is a matrix C = m × n = A + B of the same size whose elements are defined by the equations C(i,j) = A(i,j) + B(i,j).

The difference of two matrices A = m × n and B = m × n of the same size is a matrix C = m × n = A - B of the same size whose elements are defined by the equations C(i,j) = A(i,j) - B(i,j).


```
            1 2 3   1 0 0   2 2 3
С = A + B = 0 4 5 + 2 0 0 = 2 4 5
            0 0 6   3 4 1   3 4 7
```

### Matrix multiplication by scalar (mult_number). Multiplication of two matrices (mult_matrix)

```c
int s21_mult_number(matrix_t *A, double number, matrix_t *result);
int s21_mult_matrix(matrix_t *A, matrix_t *B, matrix_t *result);
```

The product of the matrix A = m × n by the number λ is the matrix B = m × n = λ × A whose elements are defined by the equations B = λ × A(i,j).

```
                1 2 3   2 4 6   
B = 2 × A = 2 × 0 4 2 = 0 8 4 
                2 3 4   4 6 8   
```

The product of A = m × k by B = k × n is a matrix C = m × n = A × B of size m × n whose elements are defined by the equation C(i,j) = A(i,1) × B(1,j) + A(i,2) × B(2,j) + ... + A(i,k) × B(k,j).

```
            1 4    1 -1  1    9 11 17   
C = A × B = 2 5  × 2  3  4 = 12 13 22
            3 6              15 15 27
```
The components of matrix C are calculated as follows:

```
C(1,1) = A(1,1) × B(1,1) + A(1,2) × B(2,1) = 1 × 1 + 4 × 2 = 1 + 8 = 9
C(1,2) = A(1,1) × B(1,2) + A(1,2) × B(2,2) = 1 × (-1) + 4 × 3 = (-1) + 12 = 11
C(1,3) = A(1,1) × B(1,3) + A(1,2) × B(2,3) = 1 × 1 + 4 × 4 = 1 + 16 = 17
C(2,1) = A(2,1) × B(1,1) + A(2,2) × B(2,1) = 2 × 1 + 5 × 2 = 2 + 10 = 12
C(2,2) = A(2,1) × B(1,2) + A(2,2) × B(2,2) = 2 × (-1) + 5 × 3 = (-2) + 15 = 13
C(2,3) = A(2,1) × B(1,3) + A(2,2) × B(2,3) = 2 × 1 + 5 × 4 = 2 + 20 = 22
C(3,1) = A(3,1) × B(1,1) + A(3,2) × B(2,1) = 3 × 1 + 6 × 2 = 3 + 12 = 15
C(3,2) = A(3,1) × B(1,2) + A(3,2) × B(2,2) = 3 × (-1) + 6 × 3 = (-3) + 18 = 15
C(3,3) = A(3,1) × B(1,3) + A(3,2) × B(2,3) = 3 × 1 + 6 × 4 = 3 + 24 = 27			
```

### Matrix transpose (transpose)

```c
int s21_transpose(matrix_t *A, matrix_t *result);
```

The transpose of matrix A is in switching its rows with its columns with their numbers retained

```
          1 4   1 2 3
A = A^T = 2 5 = 4 5 6
          3 6
```
### Minor of matrix and matrix of algebraic complements (calc_complements)
```c
int s21_calc_complements(matrix_t *A, matrix_t *result);
```

Minor M(i,j) is a (n-1)-order determinant obtained by deleting out the i-th row and the j-th column from the matrix A.

For the following matrix:

```
    1 2 3
A = 0 4 2
    5 2 1
```

The minor of the first element of the first row is:

```
M(1,1) = 4 2
         2 1

|M| = 4 - 4 = 0
```

The minors of matrix will look like this:

```
     0 -10 -20
M = -4 -14  -8
    -8   2   4
```

The algebraic complement of a matrix element is the value of the minor multiplied by -1^(i+j).

The matrix of algebraic complement will look like this:

```
      0  10 -20
M. =  4 -14   8
     -8  -2   4
```

### Matrix determinant

```c
int s21_determinant(matrix_t *A, double *result);
```

The determinant is a number that is associated to each square matrix and calculated from the elements using special formulas. \
Tip: The determinant can only be calculated for a square matrix.

The determinant of a matrix equals the sum of the products of elements of the row (column) and the corresponding algebraic complements.

Finding the determinant of matrix A by the first row:

```
    1 2 3
A = 4 5 6
    7 8 9
	
|A| = 1 × 5 6 - 2 × 4 6 + 3 × 4 5 = 1 × (5 × 9 - 8 × 6) - 2 × (4 × 9 - 6 × 7) + 3 × (4 × 8 - 7 × 5)
          8 9       7 9       7 8
|A| = 1 × (45 - 48) - 2 × (36 - 42) + 3 × (32 - 35) = -3 + 12 + (-9) = 0
|A| = 0
```

### Inverse of the matrix (inverse_matrix)

```c
int s21_inverse_matrix(matrix_t *A, matrix_t *result);
```

A matrix A to the power of -1 is called the inverse of a square matrix A if the product of these matrices equals the identity matrix.

If the determinant of the matrix is zero, then it does not have an inverse.

The formula to calculate the inverse of matrix is $`A^{-1}=\frac{1} {|A|} × A_*^T`$

The following matrix is given:

```
     2  5  7
A =  6  3  4
     5 -2 -3
```

Finding the determinant:

``` |A| = -1 ```

Determinant |A| != 0 -> matrix has an inverse.

Construction of minor matrix:

```
    -1 -38 -27
М = -1 -41 -29
    -1 -34 -24
```


The matrix of algebraic complements:

```
     -1  38 -27
М. =  1 -41  29
     -1  34 -24
```

The transpose of matrix of algebraic complements:

```
        -1   1  -1
М^T. =  38 -41  34
       -27  29 -24
```

The inverse matrix will look like this:

```
                           1  -1   1
A^(-1) =  1/|A| * M^T. = -38  41 -34
                          27 -29  24 
```


# Chapter III

## Part 1. Implementation of the matrix.h library functions

Implement basic operations with matrices (partially described [above](#matrix-operations)): create_matrix (creation), remove_matrix (cleaning and destruction), eq_matrix (comparison), sum_matrix (addition), sub_matrix (subtraction), mult_matrix (multiplication), mult_number (multiplication by number), transpose (transpose), determinant (calculation of determinant), calc_complements (calculation of matrix of algebraic complements), inverse_matrix (finding inverse of the matrix).

- The library must be developed in C language of C11 standard using gcc compiler.
- The library code must be located in the src folder on the develop branch.
- Do not use outdated and legacy language constructions and library functions. Pay attention to the legacy and obsolete marks in the official documentation on the language and the libraries used. Use the POSIX.1-2017 standard.
- When writing code it is necessary to follow the Google style for C++ ([link](https://google.github.io/styleguide/cppguide.html)).
- Make it as a static library named *s21_matrix.a* (with the s21_matrix.h header file).
- The library must be developed according to the principles of structured programming.
- Use prefix s21_ before each function.
- Prepare full coverage of library functions code with unit-tests using the Check library.
- Unit tests must cover at least 80% of each function (checked using gcov).
- Provide a Makefile for building the library and tests (with targets all, clean, test, s21_matrix.a, gcov_report).
- The gcov_report target should generate a gcov report in the form of an html page. Unit tests must be run with gcov flags to do this.
- The matrix must be implemented as the structure described [above](#matrix-structure-in-c-language).
- Verifiable accuracy of the fractional part is up to 6 decimal places.
