# Digital Logic Unit

A 2-bit logic unit that performs AND, OR, XOR, and XNOR operations
on two 2-bit inputs, with output selected via a 4:1 multiplexer.

## How It Works
The circuit takes two 2-bit inputs (A1 A0 and B1 B0) and two selector
inputs (X, Y) that choose which logic operation to perform:

| X | Y | Operation |
|---|---|-----------|
| 0 | 0 | AND       |
| 0 | 1 | OR        |
| 1 | 0 | XOR       |
| 1 | 1 | XNOR      |

## Components Used
- AND Gate IC (7408)
- OR Gate IC (7432)
- XOR Gate IC (7486)
- NOT Gate IC (7414)
- 4:1 MUX IC (74153)
- LEDs for output visualization
- Breadboard, resistors, toggle switches, 5V DC adapter

## Implementation
- Each pair of inputs (A0,B0) and (A1,B1) is processed through
  all four gates simultaneously
- A 4:1 multiplexer selects which gate output to display
  based on selector inputs X and Y
- Output is shown via LED (ON = 1, OFF = 0)

## Files
- `report.pdf` — full project report with truth tables,
   K-maps, and circuit diagrams
