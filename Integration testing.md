=======
# Integratietesting 2nd-factor

# Second Factor

# Milestone 2

#

#Integratietesting REST 2nd-factor
deze testen testen de HTTP api van de backend en mocken de TCP verbinding.

**Test_GET_CODE**

* Actie:		Stuur een GET request naar het path /code/.
* verificatie:	Er zal een status 404 not found bericht verschijnen.

**Test_GET_GENERATE_CODE**

* Actie :		Stuur een GET request naar het path "/code/generate".
* verificatie:  Er word een bericht ontvangen met daarin een kleurcode voor invoeren. 
				Daarnaast zal de status code 201 Created aanwezig zijn. 
				
**Test_GET_VERIFY_RIGHT_CODE**

* pre-actie:	1. Stuur een GET request naar het path "/code/generate".
				
			    * 2. voer de GEGENEREERDE code in op de 2nd-factor module en verzend dit naar de server.		 

* Actie :		Stuur een GET request naar het path "/code/verify".
* verificatie:	Er word een bericht ontvangen met daarin dat de code juist is. 
				Daarnaast zal de status code 202 Acceptable aanwezig zijn. 

**Test_GET_VERIFY_RIGHT_AFTER_TIMELIMIT_HAS_PASSED_CODE**

* pre-actie:*	* 1. Stuur een GET request naar het path "/code/generate".
				
				* 2. voer de GEGENEREERDE code in op de 2nd-factor module en verzend dit naar de server.		 
				
				* 3. wacht 35 seconden lang.
			 
* Actie :		Stuur een GET request naar het path "/code/verify".
* verificatie:	Er word een bericht ontvangen met daarin dat de code juist is. 
				Daarnaast zal de status code 408 Request Timeout aanwezig zijn. 

**Test_GET_VERIFY_WRONG_CODE**

* pre-actie:	voer een RANDOM code in op de 2nd-factor module en verzend dit naar de server.		 

* Actie :		Stuur een GET request naar het path "/code/verify".
* verificatie:	Er word een bericht ontvangen met daarin dat de code onjuist is. 
				Daarnaast zal de status code 406 Not Acceptable aanwezig zijn. 

**Test_GET_VERIFY_NO_CODE**

* Actie :		Stuur een GET request naar het path "/code/verify".
* verificatie: 	er zal een status 406  Not Acceptable bericht verschijnen.

**Test_POST_GENERATE_CODE**

* Actie :		Stuur een POST request naar het path "/code/generate".
* verificatie:	er zal een status 405  Method Not Allowed bericht verschijnen.

**Test_PUT_GENERATE_CODE**

* Actie :		Stuur een PUT request naar het path "/code/generate".
* Verificatie:	er zal een status 405  Method Not Allowed bericht verschijnen.

**Test_POST_VERIFY_CODE**

* Actie :		Stuur een POST request naar het path "/code/verify".
* verificatie:	er zal een status 405  Method Not Allowed bericht verschijnen.

**Test_PUT_VERIFY_CODE**

* Actie :		Stuur een PUT request naar het path "/code/verify".
* verificatie:	er zal een status 405  Method Not Allowed bericht verschijnen.		 



