# kroger\_vink.sty

LaTeX macros for Kröger-Vink notation.

## Usage
In your document preamble:

```
\usepackage{kroger_vink}
```

## Typesetting Kröger-Vink symbols
This set of macros provides a command `\kv{A}{B}{C}`. This command takes three arguments:

- `A`: Defect species, e.g. `F`.
- `B`: Defect site, e.g. `O`.
- `C`: The relative charge, e.g. `+2`.

If the relative charge is not zero (`0`), it should include a plus or minus sign (e.g. `+2` or `-1`).

The output F<sub>O</sub><sup>&times;</sup> is generated with `\kv{F}{O}{0}`.

The file includes a `\vac` command, which gives an italicised *V* for vacancies.
