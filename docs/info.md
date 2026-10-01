## How it works

This project is a purely combinational circuit built with logic gates (NOT, AND, OR, XOR and buffer). Two inputs, P (ui[0]) and Q (ui[1]), select one of four letters that is shown on a 7-segment display connected to uo[0] to uo[6] (segments a to g).

| Letter | P (ui[0]) | Q (ui[1]) |
|--------|-----------|-----------|
| D      | 0 | 0 |
| A      | 0 | 1 |
| n      | 1 | 0 |
| Y      | 1 | 1 |

Each segment is a Boolean function of P and Q:

- a = P'Q
- b = P' + Q
- c = g = 1 (always on)
- d = (P xor Q)'
- e = (PQ)'
- f = Q

## How to test

Connect a common-cathode 7-segment display to uo[0] to uo[6] (segments a to g). Set ui[0] and ui[1] to the code of the letter you want, using the table above, and the display shows that letter.

## External hardware

A common-cathode 7-segment display on uo[0] to uo[6] (the Tiny Tapeout demo board already has one).
