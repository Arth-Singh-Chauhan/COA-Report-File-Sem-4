Experiment Title:
Design and Implementation of Half Adder, Full Adder, and 4-Bit Binary Adders Using Universal Gates and Exclusive Gates in Logisim

Aim:
To design, simulate, and verify the operation of Half Adder, Full Adder, 4-Bit Binary Adder(Ripple Carry Adder) using Universal Gates(NAND/NOR) and Exclusive Gates(XOR/XNOR) in Logisim software.

Software Used:
Logisim (A graphical tool for designing and simulating digital logic circuits)

Theory:
Half Adder
A half adder is a combinational circuit that adds two single-bit binary numbers. It produces two outputs:
• Sum (S): $$S = A \oplus B$$
• Carry (C): $$C = A \cdot B$$

Full Adder
A full adder adds three single-bit binary numbers (two inputs and a carry-in). Outputs:
• Sum: $$S = A \oplus B \oplus C{in}$$
• Carry Out: $$C{out} = (A \cdot B) + (C{in} \cdot (A \oplus B))$$

4-Bit Binary Adder (Ripple Carry Adder)
A 4-bit adder chains four full adders, with the carry output of each stage connected to the carry input of the next. This allows addition of two 4-bit binary numbers, producing a 4-bit sum and a carry out.

Universal Gates
NAND and NOR gates are called universal gates because any logic function can be implemented using only NAND or only NOR gates. The adder circuits can be constructed entirely from these gates.

Exclusive Gates
XOR and XNOR gates are particularly efficient for arithmetic operations. XOR directly implements the sum function, making adder design more compact.

Procedure:
Launch Logisim and create a new project.
Design the Half Adder:
   - Place input pins for A and B.
   - Use XOR gate for Sum output.
   - Use AND gate for Carry output.
   - Connect output pins and label appropriately.
Design the Full Adder:
   - Place input pins for A, B, and Carry-in.
   - Use two XOR gates and two AND gates with an OR gate (or equivalent using universal gates).
   - Connect outputs for Sum and Carry-out.
Design the 4-Bit Adder Using Universal Gates:
   - Convert all logic gates (AND, OR, XOR) into their NAND or NOR equivalents.
   - Cascade four full adders to form a ripple carry adder.
   - Connect the carry chain and label all inputs/outputs.
Design the 4-Bit Adder Using Exclusive Gates:
   - Use XOR gates for sum generation and AND/OR gates for carry propagation.
   - Optionally, implement carry logic using XNOR where applicable.
Simulate each circuit:
   - Apply different input combinations.
   - Observe and record outputs.
Verify correctness by comparing outputs with expected truth tables.

Circuit Diagrams:
| Circuit | Screenshot |
|---------|------------|
| Half Adder | (Insert screenshot) |
| Full Adder | (Insert screenshot) |
| 4-Bit Adder (Universal Gates) | (Insert screenshot) |
| 4-Bit Adder (Exclusive Gates) | (Insert screenshot) |

Truth Tables:
Half Adder
| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

Full Adder
| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |   0  |
| 0 | 0 |  1  |  1  |   0  |
| 0 | 1 |  0  |  1  |   0  |
| 0 | 1 |  1  |  0  |   1  |
| 1 | 0 |  0  |  1  |   0  |
| 1 | 0 |  1  |  0  |   1  |
| 1 | 1 |  0  |  0  |   1  |
| 1 | 1 |  1  |  1  |   1  |

Observations:
• The half adder correctly computes the sum and carry for all input combinations.
• The full adder produces accurate results for all 8 input combinations, including carry-in.
• The 4-bit adders correctly add two 4-bit numbers, with the final carry-out indicating overflow beyond 4 bits.
• Circuits built with universal gates require more gates but demonstrate functional equivalence.
• Circuits using exclusive gates are more compact and efficient for arithmetic operations.

Result:
All designed circuits—half adder, full adder, and both 4-bit binary adders—were successfully implemented and verified in Logisim. The simulation outputs matched the expected truth table values for all test cases.

Conclusion:
This experiment demonstrated the design and working of fundamental adder circuits using both universal and exclusive gates in Logisim. The use of NAND/NOR gates proved that any combinational logic can be realized with universal gates, while XOR-based designs offered efficiency for arithmetic operations. Understanding these building blocks is essential for designing more complex arithmetic and logic units in computer architecture.
