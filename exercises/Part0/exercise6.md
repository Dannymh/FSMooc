```mermaid
  sequenceDiagram
      participant browser
      participant server
  
      browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
      activate server
      server-->>browser: 201 Created
      deactivate server
  
      Note right of browser: No reload or redirect is sent from Server. Browser adds new note via AJAX and stays on same page
```
