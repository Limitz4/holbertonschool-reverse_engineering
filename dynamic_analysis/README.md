# Dynamic Analysis and Advanced Binary Reasoning

## Overview

This project explores the behavior of compiled programs through guided reverse-engineering challenges, including constraint solving, anti-debugging, self-modifying code, and input-validation puzzles. The larger learning area combines static reasoning with runtime investigation in isolated environments.

## Challenge Map

| Artifact | Topic |
| --- | --- |
| `0-flag.txt` | Translating binary constraints into a form suitable for SAT/SMT solving |
| `1-flag.txt` | Recognizing anti-debugging checks that complicate runtime inspection |
| `2-flag.txt` | Using logical constraints and solver-based reasoning to understand binary checks |
| `3-flag.txt` | Studying self-modifying code and the difference between stored and executed instructions |
| `4-flag.txt` | Reasoning about a collection of 100 small arithmetic input-validation binaries |

## Concepts Explored

- Debugging and tracing versus non-executing, static inspection.
- Constraint-based analysis with SAT/SMT concepts such as those used by Z3.
- Program checks intended to detect or resist debugging.
- How code modification at runtime changes execution flow.
- Decomposing repetitive binary-analysis tasks into simpler checks.

## Tools Referenced by the Exercises

GDB, x64dbg, IDA/Ghidra, Z3, Python, and Pwntools are relevant to these challenge types. They are listed as learning context, **not** as tooling reproduced by the repository artifacts.

## Evidence and Limitations

Only five `*-flag.txt` verification files are committed in this directory. The source binaries, solver models, debugger traces, and automated scripts are not included, so the repository should not be interpreted as a complete executable analysis toolkit or as proof of specific automation methods.

The topics are intended for legally authorized exercises in a local VM or sandbox.
