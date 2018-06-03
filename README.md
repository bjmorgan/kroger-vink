# kroger\_vink.sty

LaTeX macros for Kröger-Vink notation.  

## Usage
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

The package includes a `\vac` command, which gives a vacancy symbol, specified in the package options (see below).

### Options

The default character for a vacany is an italic capital *V*. This can be changed by specifying the approriate package option:

```
\usepackage[uppercasevac]{kroger_vink}
```
to produce an uppercase V: *V*.

```
\usepackage[lowercasevac]{kroger_vink}
```
to produce a lowercase v: *v*.

```
\usepackage[uppercasevac]{kroger_vink}
```
to produce a square: &#9634;.

Other characters or symbols can be used if specified with the `\kvsetvacsymbol{}` command.
