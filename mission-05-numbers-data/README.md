# Mission 5 — Numbers and data

## 1. Mission title

Mission 5 — Numbers and data

## 2. Task / objective

Convert decimal, binary and hexadecimal values by hand, verify the results with Python, build a small converter and explain text encoding.

## 3. Work completed

### Task 5.1 — Convert numbers by hand

| Question | Working and answer |
|---|---|
| Decimal 13 to binary | Repeated division: 13 ÷ 2 = 6 remainder 1; 6 ÷ 2 = 3 remainder 0; 3 ÷ 2 = 1 remainder 1; 1 ÷ 2 = 0 remainder 1. Reading remainders from bottom to top: `1101` |
| Decimal 25 to binary | Repeated division: 25 → 12 remainder 1; 12 → 6 remainder 0; 6 → 3 remainder 0; 3 → 1 remainder 1; 1 → 0 remainder 1. Reading remainders upward: `11001` |
| Binary 1010 to decimal | `(1 × 2³) + (0 × 2²) + (1 × 2¹) + (0 × 2⁰) = 8 + 0 + 2 + 0 = 10` |
| Binary 1101 to decimal | `(1 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰) = 8 + 4 + 0 + 1 = 13` |
| Hexadecimal A to decimal | `A = 10 × 16⁰ = 10` |
| Hexadecimal 1F to decimal | `(1 × 16¹) + (15 × 16⁰) = 16 + 15 = 31` |
| Binary 1111 to hexadecimal | `1111₂ = 15₁₀ = F₁₆` |

### Task 5.2 — Verify using Python

| Expression tested | Result | Matches manual calculation? |
|---|---|---|
| `bin(13)` | `0b1101` | Yes |
| `bin(25)` | `0b11001` | Yes |
| `int('1010', 2)` | `10` | Yes |
| `int('1101', 2)` | `13` | Yes |
| `int('A', 16)` | `10` | Yes |
| `int('1F', 16)` | `31` | Yes |
| `hex(int('1111', 2))` | `0xf` | Yes |

### Task 5.3 — Build a number converter

Created `number_converter.py`. It uses `input()` to ask for a number, `int()` to convert the entered text to a decimal integer, `bin()` to produce binary and `hex()` to produce hexadecimal.

| Test number | Binary output | Hexadecimal output |
|---:|---|---|
| 13 | `0b1101` | `0xd` |
| 25 | `0b11001` | `0x19` |
| 42 | `0b101010` | `0x2a` |

`bin()` prefixes binary results with `0b`, and `hex()` prefixes hexadecimal results with `0x`.

### Task 5.4 — How is text stored?

- ASCII decimal code for uppercase `A`: **65**
- ASCII decimal code for lowercase `a`: **97**
- Encoding is needed because computers store bits, not characters directly. An encoding standard gives every character a numeric value so applications and devices can interpret and exchange text consistently.
- Example character outside basic ASCII: `न` (Devanagari letter) or `é`.

## 4. Commands / tools used

- Python 3 interactive shell — verified conversions with `bin()`, `int()` and `hex()`.
- `python3 number_converter.py` — ran the number converter.
- `input()` — collected the user's decimal number.
- `int()` — converted entered text to an integer.
- `bin()` and `hex()` — converted decimals to binary and hexadecimal.
- `ord()` — checked character-code values.

## 5. My understanding

Number bases represent quantities using different place values. Binary uses powers of two, decimal uses powers of ten and hexadecimal uses powers of sixteen. Text encoding converts characters into binary values; ASCII covers basic characters, while UTF-8 can represent a much wider set of characters.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- `README.md`
- `number_converter.py`
- Manual conversion working and Python verification recorded above

## 9. Commit details

- Commit message: `Build number converter and practise data representation`
- Status: Committed and pushed successfully to `main`.
