<<<<<<< HEAD
Integratietesting REST 2nd-factor

Test_GET_CODE
Actie: 		 Stuur een GET request naar het path /code/
verificatie: Er zal een status 404 not found bericht verschijnen.

Test_GET_GENERATE_CODE
Actie :		 Stuur een GET request naar het path "/code/generate"
verificatie: Er word een bericht ontvangen met daarin een kleurcode voor invoeren. 
			 Daarnaast zal de status code 201 aanwezig zijn. 
				
Test_GET_VERIFY_RIGHT_CODE
pre-actie:	 - Stuur een GET request naar het path "/code/generate"
			 - voer de GEGENEREERDE code in op de 2nd-factor module en verzend dit naar de server.		 
Actie :		 Stuur een GET request naar het path "/code/verify"
verificatie: Er word een bericht ontvangen met daarin dat de code juist is. 
			 Daarnaast zal de status code 202 aanwezig zijn. 

Test_GET_VERIFY_RIGHT_AFTER_TIMELIMIT_HAS_PASSED_CODE
pre-actie:	 - Stuur een GET request naar het path "/code/generate"
			 - voer de GEGENEREERDE code in op de 2nd-factor module en verzend dit naar de server.		 
			 - wacht 35 seconden lang
Actie :		 Stuur een GET request naar het path "/code/verify"
verificatie: Er word een bericht ontvangen met daarin dat de code juist is. 
			 Daarnaast zal de status code 408 Request Timeout aanwezig zijn. 

Test_GET_VERIFY_WRONG_CODE
pre-actie:	 - voer een RANDOM code in op de 2nd-factor module en verzend dit naar de server.		 
Actie :		 Stuur een GET request naar het path "/code/verify"
verificatie: Er word een bericht ontvangen met daarin dat de code onjuist is. 
			 Daarnaast zal de status code 406 Not Acceptable aanwezig zijn. 

Test_GET_VERIFY_NO_CODE
Actie :		 Stuur een GET request naar het path "/code/verify"
verificatie: er zal een status 406  Not Acceptable bericht verschijnen.

Test_POST_GENERATE_CODE
Actie :		 Stuur een POST request naar het path "/code/generate"
verificatie: er zal een status 405  Method Not Allowed bericht verschijnen.

Test_PUT_GENERATE_CODE
Actie :		 Stuur een PUT request naar het path "/code/generate"
verificatie: er zal een status 405  Method Not Allowed bericht verschijnen.

Test_POST_VERIFY_CODE
Actie :		 Stuur een POST request naar het path "/code/verify"
verificatie: er zal een status 405  Method Not Allowed bericht verschijnen.

Test_PUT_VERIFY_CODE
Actie :		 Stuur een PUT request naar het path "/code/verify"
verificatie: er zal een status 405  Method Not Allowed bericht verschijnen.		 

=======
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
>>>>>>> 277fa06ae6d722e3bc54b0184cbba14389c26aab
