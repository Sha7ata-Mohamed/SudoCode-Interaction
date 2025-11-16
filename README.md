# Pseudocode & Interaction – Introduction

This README explains **two core concepts** you’ll use a lot in computing:

- **Pseudocode** → how the **program thinks** (logic in plain language).
- **Interaction** → how the user and the system **talk to each other** (steps of using the system).

---

## 1. Pseudocode

### 1.1 What Is Pseudocode?

Pseudocode is a way to write the **steps of a solution** in simple, structured language without worrying about real code syntax.

- Not tied to any programming language (NOT a Coding Language).
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

```text
1. System:
   - Displays a login page with:
     - Email input field
     - Password input field
     - "Sign In" button
     - Optional: "Forgot Password?" link

2. User:
   - Clicks on the Email field.
   - Types their email address.
   - Clicks on the Password field.
   - Types their password.
   - Clicks the "Sign In" button.

3. System (Client-Side Check):
   - Checks if email field is not empty.
   - Checks if email looks like a valid format (contains "@" etc.).
   - Checks if password is not empty.

4. IF there is a problem (for example: password is empty):
   - System shows an error message under the field:
     "Password cannot be empty."
   - System does NOT send data to the server.
   - User stays on the same page.

5. ELSE (inputs look valid):
   - System sends email and password to the server.

6. Server:
   - Looks up the email in the database.
   - Compares the submitted password with the stored password.

7. IF credentials are correct:
   - Server returns success.
   - System redirects user to the dashboard/home page.
   - System displays a welcome message like:
     "Welcome back, Abdulrahman!"

8. ELSE (wrong email or password):
   - Server returns failure.
   - System stays on the login page.
   - System displays an error message:
     "Invalid email or password. Please try again."
```

---

## 3. How They Work Together

- **Pseudocode** describes the **internal logic** of the system (what decisions the program makes).
- **Interaction** describes the **external behavior** (how the user experiences those decisions).

You usually:

1. Design the **interaction flow** (what the user sees and does).
2. Write **pseudocode** for the logic behind each step.
3. Then convert the pseudocode into real code (Python, Java, etc.).
