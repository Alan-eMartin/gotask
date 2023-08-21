# GoTask - CLI Task Manager

## Description

GoTask is a Command Line Interface (CLI) based task management application. It allows users to quickly manage and track tasks without leaving the terminal. This tool aims to be lightweight, fast, and intuitive, leveraging Go's performance benefits.

## Features

### 1. Add Task

-   **Description**: Users should be able to add a task by providing a short description.
-   **Command**: `gotask add "Write MVP for GoTask"`
-   **Optional**: Due date for the task.

### 2. List Tasks

-   **Description**: List all tasks, both completed and pending.
-   **Command**: `gotask list`
-   **Optional**: Flags to filter by date, status (done/undone).

### 3. Update Task

-   **Description**: Allow users to modify an existing task, such as changing its description or due date.
-   **Command**: `gotask update [task_id] "New description"`

### 4. Complete Task

-   **Description**: Mark a task as complete.
-   **Command**: `gotask done [task_id]`

### 5. Delete Task

-   **Description**: Remove a task from the list.
-   **Command**: `gotask delete [task_id]`

### 6. Prioritize Task

-   **Description**: Highlight a task as high-priority.
-   **Command**: `gotask prioritize [task_id]`
-   **Optional**: Different priority levels (low, medium, high).

### 7. Search Task

-   **Description**: Search for tasks based on keywords in their description.
-   **Command**: `gotask search "keyword"`

## Data Storage

For the MVP, tasks can be stored in a local JSON file. Each task will have a unique ID, description, status (done/undone), priority level, and optionally, a due date.

## Non-functional Requirements

1. **Performance**: GoTask should be responsive and should not lag, even with a sizable number of tasks.
2. **Usability**: Commands should be intuitive and easy to remember.
3. **Portability**: As a CLI application, GoTask should be easily usable across various terminal emulators and OS platforms.

## Potential Extensions (Post MVP)

1. **Syncing with Cloud**: Integration with cloud services to sync tasks across devices.
2. **Notifications**: Provide notifications for tasks nearing their due date.
3. **Recurring Tasks**: Allow setting tasks that recur daily, weekly, or custom intervals.
4. **Color-Coding**: Highlight tasks based on their priority or status.
5. **Export/Import**: Export the task list to CSV/JSON and allow imports.
