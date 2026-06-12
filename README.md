# Logical Foundations Solutions

My worked solutions to **_Logical Foundations_** — volume 1 of the [Software Foundations](https://softwarefoundations.cis.upenn.edu/) series — covering functional programming in Coq, inductive proofs, constructive logic, and the formalization of a small imperative language (Imp).

## Contents

The repo is the book's chapter scripts with the exercises filled in, spanning the full core sequence — `Basics`, `Induction`, `Lists`, `Poly`, `Tactics`, `Logic`, `IndProp`, `Maps`, `ProofObjects`, `IndPrinciples`, `Rel` — plus the Imp track (`Imp`, `ImpCEvalFun`, `ImpParser`, `Extraction`, `Auto`). Exercises are complete; the only remaining `Admitted.` is the book's own `ev_even_firsttry` expository placeholder in `IndProp.v`.

## Usage

Open the `.v` files in CoqIDE, Proof General, or VsCoq and step through them. Chapters `Require` earlier ones, so compile in dependency order first, e.g.:

```bash
coqc Basics.v Induction.v Lists.v Poly.v Tactics.v Logic.v IndProp.v Maps.v ...
```

This is a circa-2018 edition of the book (it still uses `beq_nat`-era naming, before the `eqb` rename), so a contemporary Coq release (8.7–8.8) is the safest bet for replaying the proofs.

## Note

If you are taking a course that uses Software Foundations, do the exercises yourself before reading solutions.
