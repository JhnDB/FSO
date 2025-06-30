```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Server Response. 201 Created
    deactivate server
    
    Note right of browser: No reload; new list item is displayed
```