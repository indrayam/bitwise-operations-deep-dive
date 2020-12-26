# bitwise-operations-deep-dive

## Concepts
- Bitwise AND, OR, XOR and NOT
- Bitwise representation of positive and negative numbers
- 2's complement

## Bitwise Operators
- `&` (and): The binary AND operation has two inputs and one output. Always produce a 1 output if both of its inputs are 1 and will produce a 0 output if one or both of its inputs are 0.
  + 0, 0 => 0
  + 1, 0 => 0
  + 0, 1 => 0
  + 1, 1 => 1
- `|` (or): The binary OR operation has two inputs and one output. Always produce a 1 output if either of its inputs are 1 and will produce a 0 output if both of its inputs are 0.
  + 0, 0 => 0
  + 1, 0 => 0
  + 0, 1 => 0
  + 1, 1 => 1
- `^` (xor): The binary XOR (exclusive OR) operation has two inputs and one output. Always produce a 1 output if either of its inputs are 1 and will produce a 0 output if both of its inputs are 0 or 1.
  + 0, 0 => 0
  + 1, 0 => 0
  + 0, 1 => 0
  + 1, 1 => 1
- `~` (not): The binary NOT operation has one input and one output. Always produce a 1 output if its input is 0 and will produce a 0 output if its input is 1.
  + 0 => 1
  + 1 => 0
- To convert a positive number into a negative number using the **Two’s complement** representation, invert all of the bits of the number and ​add 11. Let's play with 23:

```
23    = 00000000 00000000 00000000 00010111
Inv   = 11111111 11111111 11111111 11101000
+ 1   = 00000000 00000000 00000000 00000001
Res   = 11111111 11111111 11111111 11101001
```
- The bit shifts are sometimes considered bitwise operations, because they treat a value as a series of bits rather than as a numerical quantity. In these operations the digits are moved, or shifted, to the left or right. Registers in a computer processor have a fixed width, so some bits will be "shifted out" of the register at one end, while the same number of bits are "shifted in" from the other end; the differences between bit shift operators lie in how they determine the values of the shifted-in bits.
- In an *Arithmetic shift*, the bits that are shifted out of either end are discarded. In a left arithmetic shift, zeros are shifted in on the right; in a right arithmetic shift, the sign bit (the MSB in two's complement) is shifted in on the left, thus preserving the sign of the operand.

## References
- [Bitwise AND Operation](http://www.xcprod.com/titan/XCSB-DOC/binary_and.html)
- [Bitwise OR Operation](http://www.xcprod.com/titan/XCSB-DOC/binary_or.html)
- [Bitwise XOR Operation](http://www.xcprod.com/titan/XCSB-DOC/binary_xor.html)
- [Bitwise NOT Operation](http://www.xcprod.com/titan/XCSB-DOC/binary_not.html)
- [Binary Addition](http://web.math.princeton.edu/math_alive/1/Lab1/BinAdd.html)
- [How to represent negative binary numbers](https://www.educative.io/edpresso/how-to-represent-negative-binary-numbers)
- [Signed Binary/Decimal Conversion Using the Two's Complement Representation](https://www.students.cs.ubc.ca/~cs-121/2009W1/Handouts/signed-binary-decimal-conversions.html)
