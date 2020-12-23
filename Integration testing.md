# Integratietesting 2nd-factor

# Second Factor

# Milestone 2

#

## Normale GET request sturen

Hierme wordt de GET request methode getest op verschillende aspecten. Hierbij wordt als path het IP adress van de server gebruikt gevolgd door de gespecificeerde path in de verschillende tests.

### GetGenerateCodeTest

**Instructies**
Stuur een GET request naar de path "/generatecode"

**Verwacht resultaat**
De status code moet zijn 201. Verder wordt er een array object ontvangen als response met als type "String", met daarin drie velden.

**Daadwerkelijk resultaat:**
...

### GetVerifyCodeTest

**Instructies**
Stuur een GET request naar de path "/verifycode"

**Verwacht resultaat**
De status code moet zijn 202. Verder moet er een response in het format json met als type String worden ontvangen.

**Daadwerkelijk resultaat:**
...

## Overige http request methods tests

Onderstaand worden de overige http request methoden getest.

### PostGenerateCodeTest

**Instructies**
Stuur een POST request naar de naar path "/generatecode"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...

### PutGenerateCodeTest

**Instructies**
Stuur een PUT request naar path "/generatecode"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...

### PostVerifyCodeTest

**Instructies**
Stuur een POST request naar de naar path "/verifycode"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...

### PutVerifyCodeTest

**Instructies**
Stuur een PUT request naar path "/verifycode"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...

## Ander formaat content sturen

### GetBadFormatTest

**Instructies**
Stuur een GET request met als content format "application/xml"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...

### GetBadFormatTest2

**Instructies**
Stuur een GET request met als content format "application/yaml"

**Verwacht resultaat**
De response code is 400.

**Daadwerkelijk resultaat:**
...
