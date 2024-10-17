# 📝Notes App

A simple and intuitive React application that allows users to create, update, and delete notes. This app leverages functional components and hooks to manage the state and behavior of the notes.

## Features

- **Create Notes**: Easily add new notes by filling out a title and content.
- **Update Notes**: Select an existing note to edit its title and content.
- **Delete Notes**: Remove any notes from the list with a single click.
- **Cancel Edits**: Reset the input fields and return to the note list without saving changes.

## Code Overview

### Imports

- **`useState`**: A React hook for managing state in functional components.
- **`App.css`**: The stylesheet for styling the application.
- **`updateConditionalTypeNode`**: (Unused import in the provided code.)

### Type Definition

- **`Note`**: Defines the structure of a note, which includes:
  - `id`: A unique identifier for the note.
  - `title`: The title of the note.
  - `content`: The content of the note.

### Component Structure

- **`App` Component**: Utilizes state hooks to manage:
  - **`notes`**: An array holding all the notes.
  - **`title` and `content`**: State variables for the input fields.
  - **`selectedNote`**: Tracks which note is currently selected for editing.

### Event Handlers

- **`handleNoteClick(note)`**: Sets the selected note and populates the input fields for editing.
- **`handleAddNote(event)`**: Adds a new note to the list upon form submission.
- **`handleUpdateNote(event)`**: Updates the existing note with new content.
- **`handleCancel()`**: Resets the title and content, clearing the selected note.
- **`deleteNote(event, noteId)`**: Removes a note from the list based on its ID.

### Render Method

The component renders:
- A form for adding and editing notes.
- Conditional buttons based on whether a note is being edited or a new note is being created.
- A grid displaying all notes, where each note can be clicked to edit or deleted via a button.

### Technologies Used
- React
- TypeScript
- CSS
