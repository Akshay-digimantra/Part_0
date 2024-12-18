# Exercise 0.5: SPA Loading Diagram

sequenceDiagram
participant Browser
participant Server

    Browser->>Server: GET /index.html
    Server-->>Browser: HTML file
    Browser->>Server: GET /styles.css
    Server-->>Browser: CSS file
    Browser->>Server: GET /app.js
    Server-->>Browser: JavaScript file
    Browser->>Browser: SPA initializes
    Browser->>Server: API requests (if needed)
