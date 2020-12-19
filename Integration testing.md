Integratietesting 2nd-factor

-Andere API method testen
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


- Request sturen en verbinding verbreken
Stuur een Get request naar path "/generatecode" en verbreek direct de verbinding.
Zou een 408 Request Timeout moeten geven omdat er een request is gestuurd waar geen antwoord op komt.

Stuur een Get request naar path "/verifycode" en verbreek direct de verbinding.
Zou een 408 Request Timeout moeten geven omdat er een request is gestuurd waar geen antwoord op komt.
