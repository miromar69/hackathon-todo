# Phase I – In-Memory Todo Console App (Task CRUD)

## Purpose

Build a simple command-line Todo app in Python that stores tasks in memory and supports basic CRUD operations and completion toggling.

## Data Model

Each task has:
- `id` (integer, auto-increment, unique within one run)
- `title` (string, required, 1–200 characters)
- `description` (string, optional, up to 1000 characters)
- `completed` (boolean, default: false)

## Features

1. Add Task
   - Prompt the user for a title (required) and description (optional).
   - If the title is empty, show an error and ask again.
   - Assign the next available integer `id`.

2. View Tasks
   - Show all tasks in a list.
   - For each task display: `id`, `[ ]` or `[x]` for status, and the title.
   - If there are no tasks, display a friendly message.

3. Update Task
   - Ask the user for a task `id`.
   - If the task exists:
     - Show the current title and description.
     - Ask for a new title (Enter to keep current).
     - Ask for a new description (Enter to keep current).
   - If the task does not exist, show an error message.

4. Delete Task
   - Ask the user for a task `id`.
   - If found, remove the task from the list.
   - If not found, show an error message.

5. Toggle Complete / Incomplete
   - Ask the user for a task `id`.
   - If found, flip the `completed` flag:
     - If it was false, set to true.
     - If it was true, set to false.
   - Show a confirmation message.
   - If not found, show an error.

## User Interface Flow

- When the program starts, show a text menu in a loop:

  1. Add task
  2. View tasks
  3. Update task
  4. Delete task
  5. Toggle complete
  0. Exit

- After completing any action, the menu is shown again until the user chooses `0` to exit.
- Handle invalid menu choices with a clear message and show the menu again.

## Non-Functional Requirements

- Use standard Python 3 only (no external libraries).
- Keep the code simple and readable.
- Handle invalid input gracefully (for example non-numeric IDs).
