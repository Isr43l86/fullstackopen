sequenceDiagram
participant browser
participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    Note right of browser: The browser will send the user input to the server as JSON
    
    server-->>browser: Status code 201
    deactivate server
