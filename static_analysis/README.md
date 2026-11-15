# Static Analysis in Reverse Engineering

## Overview

Static analysis examines executable files without running them. This set of guided exercises explores how to inspect strings, follow program logic, interpret assembly, and reason about obfuscated validation algorithms using decompilers and disassemblers.

## Exercise Topics

| Artifact | Challenge theme |
| --- | --- |
| `0-flag.txt` | Extracting readable strings and identifying potentially meaningful embedded data |
| `1-flag.txt` | Reviewing the logic of a security-relevant compiled C program |
| `2-flag.txt` | Understanding and optimizing an inefficient decryption algorithm |
| `3-flag.txt` | Analyzing mathematical obfuscation and collisions in an input-validation routine |
| `4-flag.txt` | Interpreting raw assembly instructions and reconstructing high-level behavior |

## Analysis Concepts

- File inspection, readable strings, and executable layout.
- Disassembly, decompilation, and control-flow reasoning.
- Function identification, cross-references, and input-validation logic.
- The relationship between arithmetic transformations and obfuscated data.
- Complexity analysis when an algorithm makes straightforward processing impractical.

## Typical Tooling

The exercise brief covers tools such as `strings`, Ghidra, IDA, Radare2, and other binary inspection utilities. These are **relevant analysis tools**, not a claim that every tool was used or automated by files in this folder.

## Repository Evidence

The five text files contain guided challenge verification results. The target executables, tool sessions, decompilation exports, and solution scripts are **not** committed here. Accordingly, this README describes the assessed topics without presenting the flags as working analysis programs.

## Defensive Perspective

Static review helps defenders assess unknown software safely before execution, identify suspicious hardcoded material, and select functions for follow-up testing in a controlled environment.
