# Pseudocode & Interaction – Introduction

This README explains **two core concepts** you’ll use a lot in computing:

- **Pseudocode** → how the program *thinks* (logic in plain language).
- **Interaction** → how the user and the system *talk* to each other (steps of using the system).

---

## 1. Pseudocode

### 1.1 What Is Pseudocode?

Pseudocode is a way to write the **steps of a solution** in simple, structured language without worrying about real code syntax.

- Not tied to any programming language.
- Focuses on **logic** instead of details like `;`, `{}`, etc.
- Used to plan the algorithm **before** writing actual code.

### 1.2 Example: Login Check (Pseudocode)

**Goal:** Ask for username and password, then check if they are correct.

```text
START

DISPLAY "Enter username:"
READ username

DISPLAY "Enter password:"
READ password

IF username = "admin" AND password = "1234" THEN
    DISPLAY "Login successful. Welcome!"
ELSE
    DISPLAY "Login failed. Try again."
END IF

END
