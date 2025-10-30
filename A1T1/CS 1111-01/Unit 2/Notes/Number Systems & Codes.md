## Number Systems
Successive division is used to convert base 10 numbers into other number bases. The method converts numbers in different bases to decimal by relying on the fact that each digit/bit is multiplied by its base to a power corresponding to its position.

The formula for that is as follows:
$$(X_3 X_2 X_1 X_0)_b = X_3 b^3 + X_2 b^2 + X_1 b^1 + X_0 b^0$$
where $X_y$ is the orbit (digit) ($X$) and its position ($y$)
	$b$ is the base

Octal to binary conversion involves switching each octal digit for its binary equivalent as a 3-digit number. Zero's ar the start of the whole number or at the end of the decimal can be ignored.

When converting from binary to octal, starting from the least significant bit, divide into groups of 3 bits and convert bit groups. You should pad the decimal with zeroes till you have 3 bits in the last decimal group. 

Hexadecimal conversions work the same as octal except the bit groups have a size of 4.

## Number Systems II
Every number (or numeration) system is defined by a base (or radix), which is a collection of distinct symbols. In a positional number system, the value of a number depends on teh place occupied by each of its digits in the representation.

The binary code obtained for a positive number is called a natural binary code. The coefficients or numbers (0 & 1) used in the binary representation of a number are called bits. The rightmost bit is called the least-significant bit (LSB) while the leftmost bit is the most significant bit (MSB). 

The Arithmetic and Logic Unit manipulates binary numbers or words with a fixed number of bits.

A byte is an 8-bit word. In practice, the bits 0 and 1 are represented by voltage or current levels. The two regions in the figure above are separated by a forbidden region where the logical level is undefined. 

Logical states may be assigned to regions based on positive logic ($V_H\rightarrow1, V_L\rightarrow0$) or negative logic ($V_H\rightarrow0,V_L\rightarrow1$).
$$
\begin{aligned}
N_{10} &= b_{n-1} B^{n-1} + ... + b_2 B^2 + b_1 B_1 + b_0 B^0 \\
&= \sum_{i = 0}^{n-1} b_i B^i
\end{aligned}
$$

where $B\ge2$. Thus the decimal number $N$ is represented in radix $B$ with $n$ digits, $b_{n-1} ... b_2 b_1 b_0$.

Using $n$ digits in a radix $B$ numeration, we can code the decimal numbers from 0 to $B^n-1$. Explaining further, 3 digits in base 2 can go up to 7. $2^3-1$ or 2 digits in base 16 can go up to $255(FF)$. $16^2-1$.

For an integer represented by $n$ digits with a radix $B$, the formulas for conversion are as follows:
$$
\begin{align}
(b_{n-1} b_{n-2} ... b_2 b_1 b_0)_B &= \sum_{i=0}^{n-1} b_i B^i \\
&= b_{n-1} B^{n-1} + ... + b_2 B^2 + b_1 B^1 + b_0 B^0 \\
&= b_0 + B(b_1 + B(b_2 + B(... + B(b_{n-2} + B b_{n-1})...))) \\
&= N_{10}
\end{align}
$$
To represent a 8421-type binary-coded decimal (BCD) number, each digit must be replaced by its equivalent 4-bit binary. With n bits, we can represent the decimal numbers between 0 and $10^{n/4}-1$  in BCD. 8421 is not the only type of BCD code but is pretty popular.

## Data Representation
A code is necessary to manipulate and transfer alphanumeric data.

### Gray Code
Also known as reflected binary code, it is a non-weighted code, as it does not ascribe a specific weight to each bit position. It is not used in arithmetic calculations.

In Gray code representation, only a single bit changes value between the transition from one code to the next (sequentially). When converting to Gray from binary, note:
- the MSBs are the same.
- starting left, add each adjacent pair of binary bits to get the next Gray bit.
$(11001)_2 \Rightarrow (10101)_{Gray}$

To convert from Gray to binary, MSB rule applies. Then for each binary bit recorded, add to the next Gray bit to get the next binary bit. 

Gray code is used in Karnaugh maps and the design of logic circuits. Also used in rotary encoders where the predisposition to errors increases with the number of bits that change logical states between two consecutive positions.

### ASCII Code
American Standard Code for Information Exchange has 7 bits allowing for the representation of 27 - 128 symbols. ASCII code contains 34 characters used to define teh format of information and the space between data and to control the transmission and reception of symbols.

### Other Codes
- EBCDIC (Extended BCD Interchange Code) is an 8-bit code.
- ANSI (American National Standard Institute) allows for the representation of alphabetic letters from many languages.
- UTF-8, UTF-16, UTF-32, Unicode represents each character in a unique way by a number. It covers symbols used in most languages.

## Coding for the Modern Era
Around the commencement of the computer age in the 60's, EBCIDIC (IBM) and ASCII (every other manufacturer) were the two main rival schemes.

ANSI built on ASCII and has different code pages for different languages. The computer must know which code page is in use to interpret ANSI correctly.

Unicode is currently becoming the standard for many purposes. It is a much larger set including not only characters from the non-Latin alphabets like Greek, Russian and Arabic, but even non-alphabetic languages like Japanese and Chinese. UTF-8 allows the ASCII character set to be represented as it traditionally was in 8-bits. 8-bits and not 7 because most computers operate with multiples of 8-bits.