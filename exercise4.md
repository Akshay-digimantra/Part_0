# Exercise 0.4: New Note Diagram

sequenceDiagram
participant Browser
participant Server
participant Database

    Browser->>Server: POST /api/notes (note content)
    Server->>Database: Save the note
    Database-->>Server: Success response
    Server-->>Browser: 201 Created
    Browser->>Browser: Update UI
