# VHDL_Karatsuba

In these descriptons I implemented a version of the Karatsuba multiplication which is applied to calculate with extremely large numbers in O(N^1.5) time, N being the length of the multiplicands. In this special case one of the multiplicands is extra large, the other is short, because in the Montgomery multiplication, described in a different repository of mine, it can be seen, that only one of the multiplicands is extra large, the other is maximally as wide as the numbeer base used in that particular algorithm.

This current implementation was created to test how the bit widths of storage elements change during the recursive steps of the Karatsuba multiplication, and for estimation purposes on how the number of multipliers and halving steps change with respect to input sizes. Although this implementation is functional and synthesizable, it creates one huge asynchronous multiplier, that is not yet practical, and needs further optimization.
