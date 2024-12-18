# Exercise 0.6: New Note in SPA

sequenceDiagram
participant Browser
participant Server
participant Database

    Browser->>Server: POST /api/notes (note content)
    Server->>Database: Save note
    Database-->>Server: Success response
    Server-->>Browser: 201 Created (with note data)
    Browser->>Browser: Update UI dynamically
