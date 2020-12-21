Integratietesting 2nd-factor

- Normale GET request sturen

Stuur een GET request naar de path "/generatecode"
Zou een 200 OK status code terug moeten krijgen.

Stuur een GET request naar de path "/verifycode"
Zou een 200 OK status code terug moeten krijgen.


- Andere API method testen

Stuur een POST request naar de naar path "/generatecode"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen POST requests af kan handelen, alleen GET requests.

Stuur een PUT request naar path "/generatecode"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen PUT requests af kan handelen, alleen GET requests.

Stuur een POST request naar de naar path "/verifycode"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen POST requests af kan handelen, alleen GET requests.

Stuur een PUT request naar path "/verifycode"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen PUT requests af kan handelen, alleen GET requests.


- Ander formaat content sturen

Stuur een GET request met als content format "application/xml"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen XML format kan afhandelen, alleen JSON.

Stuur een GET request met als content format "application/yaml"
Zou een 400 Bad Request code terug moeten krijgen omdat de API geen YAML format kan afhandelen, alleen JSON.