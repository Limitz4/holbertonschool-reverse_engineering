# Reverse Engineering Fundamentals - ELF Inspection

## Overview

This project introduces binary inspection using Linux command-line utilities. It focuses on recognizing ELF executables, reading their headers, inspecting section metadata, and identifying dynamically linked libraries without needing the program's source code.

## Project Files

| File | Purpose |
| --- | --- |
| `get_entry_point.sh` | Validates an input file and uses `readelf` to inspect the ELF magic bytes, class, byte order, and entry-point address |
| `command.txt` | Records the `readelf -S` command used for section enumeration |
| `size.txt` | Stores the reported size of an identified unusual section from the exercise |
| `external_library.txt` | Records a library dependency identified during binary inspection |

## ELF Header Inspection

The Bash utility accepts an ELF file path as its first argument. It checks for a missing path, verifies that the file exists, checks that the file type is ELF, and extracts selected header fields with `readelf`.

```bash
./get_entry_point.sh ./target_binary
```

**Dependency note:** `get_entry_point.sh` sources a local `messages.sh` helper to format the output. That helper is referenced by the script but is **not currently included in this repository directory**; the command above therefore requires the helper to be provided before successful execution.

## Topics Practiced

- ELF headers and executable metadata.
- Entry points and the differences between 32-bit/64-bit and byte-order representations.
- Section enumeration with `readelf` or `objdump`.
- Linking and shared-library dependencies.
- File validation and argument handling in shell scripts.

## Why This Matters

Initial binary inspection can reveal file-format inconsistencies, uncommon sections, and unexpected dependencies that warrant more detailed analysis. The supporting text files record specific exercise answers; they are not substitutes for the original target binary or a full investigation report.

All inspection activities are intended for local, authorized analysis environments.
