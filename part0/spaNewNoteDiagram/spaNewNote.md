```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: {"message":"note created"}
    deactivate server

    Note right of browser: The browser starts executing the JavaScript code
    Note right of browser: It updates the notes list, redraw the UI, and then send the new note data to the server
```
