# Mission 5: Numbers and Data

## Objective

To understand different number systems, convert values between decimal, binary, and hexadecimal, verify conversions using Python, build a number converter, and learn how computers store text using character encoding.

---

## Task 5.1: Convert Numbers by Hand

I practised converting numbers between decimal, binary, and hexadecimal systems.

### Manual Conversions

**1. Decimal 13 to Binary**

Repeated division by 2:

| Division | Quotient | Remainder |
|---|---:|---:|
| 13 ÷ 2 | 6 | 1 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

Reading the remainders from bottom to top:

`13 (decimal) = 1101 (binary)`

**2. Decimal 25 to Binary**

| Division | Quotient | Remainder |
|---|---:|---:|
| 25 ÷ 2 | 12 | 1 |
| 12 ÷ 2 | 6 | 0 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

`25 (decimal) = 11001 (binary)`

**3. Binary 1010 to Decimal**

= 1 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰

= 8 + 0 + 2 + 0

= **10**

**4. Binary 1101 to Decimal**

= 1 × 2³ + 1 × 2² + 0 × 2¹ + 1 × 2⁰

= 8 + 4 + 0 + 1

= **13**

**5. Hexadecimal A to Decimal**

A = 10

Therefore, A (hexadecimal) = **10 (decimal)**

**6. Hexadecimal 1F to Decimal**

F = 15

= 1 × 16¹ + 15 × 16⁰

= 16 + 15

= **31**

**7. Binary 1111 to Hexadecimal**

1111 (binary) = 8 + 4 + 2 + 1 = 15

15 in hexadecimal is F.

Therefore, `1111 (binary) = F (hexadecimal)`.

### Summary of Conversions

| Conversion | Result |
|---|---|
| Decimal 13 → Binary | 1101 |
| Decimal 25 → Binary | 11001 |
| Binary 1010 → Decimal | 10 |
| Binary 1101 → Decimal | 13 |
| Hexadecimal A → Decimal | 10 |
| Hexadecimal 1F → Decimal | 31 |
| Binary 1111 → Hexadecimal | F |

---

## Task 5.2: Verify Using Python

I used Python's built-in functions to verify the manual conversions.

### Functions Used

- `bin()` converts an integer into binary.
- `hex()` converts an integer into hexadecimal.
- `int()` converts a number represented as a string into an integer using the specified base.

### Python Expressions and Results

| Expression | Result |
|---|---|
| `bin(13)` | `0b1101` |
| `bin(25)` | `0b11001` |
| `int("1010", 2)` | `10` |
| `int("1101", 2)` | `13` |
| `int("A", 16)` | `10` |
| `int("1F", 16)` | `31` |
| `hex(15)` | `0xf` |

All the results match the corresponding manual conversions.

### What I Learned

- Python provides built-in functions for number conversion.
- The prefix `0b` represents binary.
- The prefix `0x` represents hexadecimal.
- The second argument of `int()` specifies the base of the input number.

---

## Task 5.3: Build a Small Number Converter

I created a Python program named `number_converter.py` that accepts a decimal number and displays its binary and hexadecimal representations.

### Program Code

```python
# Decimal to Binary and Hexadecimal Converter

number = int(input("Enter a decimal number: "))

binary = bin(number)
hexadecimal = hex(number)

print("Decimal:", number)
print("Binary:", binary)
print("Hexadecimal:", hexadecimal)
```

### Sample Test Cases

**Test 1: Input = 13**

```text
Enter a decimal number: 13
Decimal: 13
Binary: 0b1101
Hexadecimal: 0xd
```

**Test 2: Input = 25**

```text
Enter a decimal number: 25
Decimal: 25
Binary: 0b11001
Hexadecimal: 0x19
```

**Test 3: Input = 31**

```text
Enter a decimal number: 31
Decimal: 31
Binary: 0b11111
Hexadecimal: 0x1f
```

### What I Learned

- How to take integer input using `input()` and `int()`.
- How to use `bin()` and `hex()` for number conversion.
- How to display converted values using `print()`.
- How to create and execute a simple Python program.

---

## Task 5.4: How Is Text Stored?

Computers store text using numerical representations of characters. Character encoding standards help computers represent and interpret text consistently.

### 1. ASCII Codes

ASCII stands for American Standard Code for Information Interchange.

It assigns numerical values to letters, digits, and symbols.

- Uppercase A = 65
- Lowercase a = 97

### 2. Why Are Encoding Standards Needed?

Computers store information in binary form. Encoding standards assign numerical representations to characters so that computers can store, interpret, and exchange text consistently.

### 3. Character Outside Basic ASCII

Examples include:

- ₹ (Indian Rupee symbol)
- अ (Devanagari character)
- 😊 (Emoji)

These characters are supported by Unicode and can be represented using UTF-8 encoding.

### What I Learned

I understood that text is also stored as numerical data. ASCII represents a basic set of characters, while Unicode supports characters from many languages and additional symbols. UTF-8 is a widely used Unicode encoding format.

---

## Overall Learning

Through this mission, I learned about decimal, binary, and hexadecimal number systems and how to convert values between them.

I practised manual conversions and verified the results using Python's built-in functions. I also created a small number converter program and learned how computers represent text using ASCII and Unicode encoding.

## Difficulties Faced

- Understanding the different number systems and their bases.
- Converting binary and hexadecimal values manually.
- Understanding how Python's built-in conversion functions work.
- Understanding how characters are represented as numerical values.

## Tools Used

- Python 3
- Visual Studio Code
- macOS Terminal
- Git and GitHub

## Conclusion

This mission helped me understand how computers represent numbers and text internally. I gained practical experience with number conversions, Python programming, and character encoding.

