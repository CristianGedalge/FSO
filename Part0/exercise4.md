```mermaid
sequenceDiagram
   participant browser
   participant server

   Note right of browser: This browser calling the POST method when clicking the button

   browser->>server POST https://studies.cs.helsinki.fi/exampleapp/notes
   activate server
   server->>browser: [{the data entered with its date}]
   deactivate server

   Note right of browser: Only the written note is shown in the browser
```