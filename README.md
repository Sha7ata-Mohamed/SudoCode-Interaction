# Pseudocode & Interaction – Introduction

This README explains **two core concepts** you’ll use a lot in computing:

- **Pseudocode** → how the program _thinks_ (logic in plain language).
- **Interaction** → how the user and the system _talk_ to each other (steps of using the system).

---

## 1. Pseudocode

### 1.1 What Is Pseudocode?

Pseudocode is a way to write the **steps of a solution** in simple, structured language without worrying about real code syntax.

- Not tied to any programming language (NOT a coding language).
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
```

---

## 2. Interaction

### 2.1 What is Interaction?

In computing, interaction is the **step-by-step** **communication** between a user and a system (like a website or app).

- The user performs an action → click, type, tap.
- The system responds → show a message, open a new page, save data.
- Good interaction is:
  - Clear
  - Predictable
  - Easy to use

---

### 2.2 Example: Login Page Interaction Flow

Here’s how a user interacts with a login page, step by step:

1. The system displays a login form with:
   - Email field
   - Password field
   - "Sign In" button

2. The user types their email and password.

3. The user clicks the "Sign In" button.

4. The system checks:
   - Is the email format valid?
   - Is the password field not empty?

5. IF there is a problem:
   - The system shows an error message
     (e.g., "Password cannot be empty.")
   ELSE
   - The system sends the data to the server.

6. The server checks if the credentials are correct.

7. IF the credentials are correct:
   - The system redirects the user to the dashboard.
   - The system shows: "Welcome back!"
   ELSE
   - The system keeps the user on the login page.
   - The system shows: "Invalid email or password."

---

## 3. How They Work Together

- **Pseudocode** describes the **internal logic** of the system (what decisions the program makes).
- **Interaction** describes the **external behavior** (how the user experiences those decisions).

You usually:

1. Design the **interaction flow** (what the user sees and does).
2. Write **pseudocode** for the logic behind each step.
3. Then convert the pseudocode into real code (Python, Java, etc.).
