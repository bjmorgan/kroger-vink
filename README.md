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
to produce an uppercase *V*.

```
\usepackage[lowercasevac]{kroger_vink}
```
to produce a lowercase *v*.

```
\usepackage[squarevac]{kroger_vink}
```
to produce a square: &#9634;.

Other characters or symbols can be used if specified with the `\kvsetvacsymbol{}` command.

### Variable or placeholder defects

If the defect species A is a variable placeholder the command `\kvv{A}{B}{C}` can be used to typeset 
an italicised <i>A</i> symbol, e.g. for a generic <i>M</i><sup>3+</sup> cation occupying a lithium site 
`kvv{M}{Li}{+2}`.
