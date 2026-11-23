# CPUT Sports Hub — Login Validator (C)

A C program that simulates a welcome screen for the CPUT Sports Hub. It prompts the
user for a username and password, then validates both against login rules.

## 🎯 What It Demonstrates

- **Pointer-based string validation** — a custom `contains()` function that scans a
  string for a substring (equivalent to `strstr()`), implemented manually with pointers
  and indices.
- **Password policy enforcement** — minimum length, at least one digit, and at least
  one special character using `<ctype.h>`.
- **Clean function separation** — validation logic lives in its own functions, called
  from `main`, with no global state.

## 📋 Login Rules

| Field    | Requirement                                              |
|----------|----------------------------------------------------------|
| Username | Must contain the domain `@mycput.ac.za`                  |
| Password | At least 8 characters, with ≥1 digit and ≥1 special char |

## 🚀 How to Run

```bash
gcc main.c -o sports_hub
./sports_hub
