## Machine learning book club

It's a club, not a class!
Contents

zach_notes_chapter_1.pdf is a nice visual reference for chapter 1 vocabulary and concepts.

chapter_1_exercises.md contains our collaborative solutions/discussion for the chapter exercises.

ryan_chapter_1_notes.md contains text reference notes and some examples.
Notation Conventions

The VMLS book uses the following notation conventions:
lower-case letters for vector variables.
Greek letters for number variables (scalars). See https://en.wikipedia.org/wiki/Greek_alphabet for reference.
Other resources might use a bold font for vector variables
Some other texts specify vectors by writing arrows above the variable name.
There is no one standard notation, sadly.
Python Guides

https://ses.library.usyd.edu.au/handle/2123/21370

## chapter_1_python_companion.ipynb is a numpy intro to chapter 1.

## Fundamental Properties of Vectors

Vector addition is commutative, meaning a + b = b + a

Vector addition is associative (a + b) + = a + (b + c)

a + 0 = 0 + a = a. Adding the zero vector has no effect.

a - a = 0. Subtracting a vector from itself yields zero.

Scalar multiplication is commutative. 3 * a = a * 3.

Scalar multiplication is associative. If a is a vector then (3*4)*a = 3(4 * a)

Left distributive property of scalar-vector multiplication is (3 + 4) * a = 3a + 4a

Inner products have the following properties:

Commutative property a.dot(b) = b.dot(a)

Associativity with scalar multiplication (3a).dot(b) = 3(a.dot(b))

Distributivity with vector addition (a + b).dot(c) = a.dot(c) + b.dot(c)

## Now We Know (CAUTION)

Don't confuse math notation with programming syntax!
Our vector notation in math is a = (1, 2, 3) or b = (4.2, 10, -11, 17.2).
Vectors index from 1 and not zero (like many programming languages)
The math notation (a, b) means a stacked vector of a and b. A stacked vector means a one dimensional vector that is the elements of a followed by the elements of b. If a = (1,2) and b = (3, 4) then the notation (a, b) means the vector (1, 2, 3, 4).
Two vectors are said to be equal if they are of the same size and and each of the corresponding entries is the same (at each index).
We cannot add, subtract, or take the dot-product of vectors of differing lengths. It's not valid.
Subvector notation is inclusive of the beginning and ending index (unlike some programming languages).
Resources:

http://vmls-book.stanford.edu/ is the full text of the VMLS book.

https://www.3blue1brown.com/essence-of-linear-algebra-page is a wonderful video series that goes into the esssence of linear algebra.

