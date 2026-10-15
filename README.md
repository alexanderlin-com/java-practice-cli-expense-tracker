# CLI Expense Tracker

Build a command-line Java application for tracking personal expenses.

The purpose of this project is not to follow a provided architecture or copy a finished implementation. The goal is to practice turning requirements into smaller responsibilities, methods, classes, and implementation steps.

You should decide the structure of the program yourself.

---

## Version 1 Requirements

The user must be able to:

- Record an expense
- View all recorded expenses
- View their total spending
- Exit the program

Expenses only need to exist while the program is running. Closing the program may erase all data.

Each expense should contain:

- An amount
- A category
- A description
- A date

The program should repeatedly present the user with available actions until they choose to exit.

Invalid input should not normally crash the program. Handle obvious user mistakes reasonably.

---

## Version 2 Requirements

Add the ability to:

- Delete an expense
- Filter expenses by category
- View spending totals for a specific category

Categories should come from a defined set rather than arbitrary free-form strings.

---

## Version 3 Requirements

Add persistence.

When the program closes, expenses should be saved to disk.

When the program starts again, previously saved expenses should be restored automatically.

Use a simple text-based file format. Do not use a database or external serialization library for this version.

---

## Version 4 Requirements

Add automated tests for the important program behavior.

Tests should focus on application logic rather than console output.

At minimum, verify behavior involving:

- Recording expenses
- Deleting expenses
- Calculating total spending
- Filtering by category
- Invalid or edge-case inputs

---

## Constraints

Do not use Spring.

Do not use a database.

Do not use AI to generate the project's architecture, classes, methods, or finished implementations.

AI may be used to:

- Explain Java concepts
- Explain compiler errors
- Explain APIs or standard-library features
- Review code you already wrote
- Point out design problems
- Ask questions that help you reason through a problem
- Give progressively stronger hints after you have attempted a solution

The main program entry point should not contain the entire application.

Prefer small responsibilities over one giant method.

Do not create abstractions merely because they sound professional. Add structure when the requirements give you a reason for it.

---

## Definition of Done

The final program should be usable entirely from the command line.

A user should be able to start the application, manage expenses, exit, restart the application, and continue working with previously saved data.

The application should have automated tests covering its important business logic.

The code should be organized well enough that adding a new requirement does not require rewriting the entire program.

---

## Development Rule

Before implementing a feature, break it down until each remaining task is concrete enough that you understand what code you are trying to write.

Do not begin with:

> "How do I build an expense tracker?"

Keep decomposing until the questions become things like:

> "How do I store this information?"

> "How do I find one item?"

> "How do I calculate this value?"

> "How do I validate this input?"

> "Which part of the program should be responsible for this behavior?"

When the next step becomes boring and specific, implement it.