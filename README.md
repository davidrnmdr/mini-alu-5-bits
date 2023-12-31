# 5 Bits Mini ALU

Welcome to my mini CPU brain, a mini Arithmetic Logic Unit (ALU) made in WiRedPanda 4.10, a logic circuits simulator developed by students of my university.

![Compiled ALU](https://i.imgur.com/DAjI05J.png)

This ALU performs 11 operations with two (or one) operators up to 5 bits:

| Op Code<sub>10</sub> | Op Code<sub>2</sub> | Operation |
| -------- | ------- | ------- |
| 0 | 0000 | A - B |
| 1 | 0001 | A = B |
| 2 | 0010 | A > B |
| 3 | 0011 | A < B |
| 4 | 0100 | A + B |
| 5 | 0101 | A ∧ B |
| 6 | 0110 | A ∨ B |
| 7 | 0111 | A ⊻ B |
| 8 | 1000 | A' |
| 9 | 1001 | B' |
| 10 | 1010 | A x B |

Internally, it is made by recursively stacking together 5 1-bit-ALUs and some 16x1 multiplexers. Although we got 11 available operations, a 16x1 MUX is needed because, as we know, the immediate smaller standard MUX is 8x1 which is insufficient to select our 11 possibilities. In the bellow image we can se the inside of it:

![ALU](https://i.imgur.com/q0xqgGu.png)



