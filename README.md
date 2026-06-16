

# Income Tax Calculator (C)

A simple command-line Income Tax Calculator written in C that calculates the total tax payable based on a progressive tax slab system.

## Features

- Calculates income tax based on predefined tax slabs.
- Simple and lightweight C program.
- Beginner-friendly implementation using conditional statements.
- Runs directly in the terminal.

## Tax Slabs

| Annual Income (₹) | Tax Rate |
|-------------------|----------|
| Up to ₹2,50,000 | 0% |
| ₹2,50,001 – ₹5,00,000 | 5% |
| ₹5,00,001 – ₹10,00,000 | 20% |
| Above ₹10,00,000 | 30% |

### Tax Calculation Logic

- No tax for income up to ₹2,50,000.
- 5% tax on income exceeding ₹2,50,000 up to ₹5,00,000.
- 20% tax on income exceeding ₹5,00,000 up to ₹10,00,000.
- 30% tax on income exceeding ₹10,00,000.

## Example

### Input

```text
Enter income:750000
```

### Output

```text
The total tax amount is 62500
```

### Calculation

For an income of ₹7,50,000:

- First ₹2,50,000 → No tax
- Next ₹2,50,000 → 5% = ₹12,500
- Remaining ₹2,50,000 → 20% = ₹50,000

**Total Tax = ₹62,500**

## Getting Started

### Prerequisites

- GCC Compiler or any C compiler

### Compilation

```bash
gcc income_tax_calculator.c -o tax_calculator
```

### Run

```bash
./tax_calculator
```

## Project Structure

```text
.
├── income_tax_calculator.c
└── README.md
```

## Code Overview

The program:

1. Takes annual income as input from the user.
2. Determines the applicable tax slab.
3. Calculates tax progressively based on the slab rates.
4. Displays the total tax payable.

## Limitations

- Uses integer data types, which may lead to loss of precision in tax calculations.
- Does not include tax rebates, cess, or deductions.
- Based on fixed tax slabs coded directly into the program.

## Future Improvements

- Use `float` or `double` for more accurate calculations.
- Add support for deductions and exemptions.
- Compare old and new tax regimes.
- Create a menu-driven interface.
- Add input validation.

## License

This project is open-source and available under the MIT License.

## Author

Created as a learning project in C programming.
