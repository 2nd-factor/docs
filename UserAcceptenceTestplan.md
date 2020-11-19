# User Acceptance Test

# Second Factor

# Milestone 2

## Login met gebruikersnaam en wachtwoord
*Hiermee testen we de requirements van: in te vullen velden bij 'gebruikersnaam' en 'wachtwoord', het verzenden van inloggegevens met een log-in knop, het tonen van een boodschap bij invoer van foutieve gegevens (op diverse manieren), het tonen van een kleurencode bij correcte login*

### Test 1

**Instructie:**
De gebruiker vult correcte gebruikersnaam en wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een kleurencombinatie te zien om in te voeren op de Arduino in te voeren.

**Daadwerkelijk resultaat:**
...


### Test 2

**Instructie:**
De beheerder vult een correcte gebruikersnaam en wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De beheerder krijgt een kleurencombinatie te zien om in te voeren op de Arduino in te voeren.

**Daadwerkelijk resultaat:**
...


### Test 3

**Instructie:**
De gebruiker vult een incorrecte gebruikersnaam en een correct wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 4

**Instructie:**
De beheerder vult een incorrecte gebruikersnaam en wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De beheerder krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 5

**Instructie:**
De gebruiker vult een correcte gebruikersnaam en een incorrect wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 6

**Instructie:**
De beheerder vult een correcte gebruikersnaam en een incorrect wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De beheerder krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 7

**Instructie:**
De gebruiker vult een incorrecte gebruikersnaam en een correct wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 8

**Instructie:**
De beheerder vult een incorrecte gebruikersnaam en een correct wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 9

**Instructie:**
De gebruiker of beheerder vult alleen een gebruikersnaam in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...


### Test 10

**Instructie:**
De gebruiker of beheerder vult alleen een wachtwoord in, klikt vervolgens op de log-in knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect username or password".

**Daadwerkelijk resultaat:**
...



## Kleuren verificatie na succesvolle log-in met user info
*Hiermee testen we de requirements van: een kleuren-code die max seconden geldig is, de welkomsboodschap op gebruikers- en beheerderspagina's, verificatie van kleurencombinatie in de backend, het invoeren van de kleuren-code op de Arduino, gebruik van de knoppen op de Arduino (kleuren, verzendknop, resetknop).*

### Test 1

**Instructie:**
De gebruiker of beheerder vult het correcte gebruikersnaam en wachtwoord in, klikt vervolgens op de log-in knop. Ze wachten 30 seconden zonder iets in te vullen op de Arduino.

**Verwacht resultaat:**
De website ververst en toont een nieuw gegenereerde kleurcode.

**Daadwerkelijk resultaat:**
...


### Test 2

**Instructie:**
De gebruiker vult na inloggen de getoonde kleuren correct in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont de gebruikerspagina met een welkomsboodschap.

**Daadwerkelijk resultaat:**
...

## Test 3

**Instructie:**
De beheerder vult na inloggen de getoonde kleuren correct in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont de beheerderspagina met een welkomsboodschap.

**Daadwerkelijk resultaat:**
...



### Test 4

**Instructie:**
De gebruiker vult de getoonde kleuren verkeerd in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont een foutmelding 'verkeerde kleurcode' en toont een nieuw gegenereerde kleurcode.

**Daadwerkelijk resultaat:**
...


### Test 5

**Instructie:**
De gebruiker vult de getoonde kleuren verkeerd in op de Arduino, drukt op de resetknop en vult daarna de juiste kleurencombinatie in.
Hierna drukt de gebruiker op de verzendknop.

**Verwacht resultaat:**
De website toont de gebruikerspagina met een welkomsboodschap.

**Daadwerkelijk resultaat:**
...



## Gebruikerspagina
*Hiermee testen we de requirements van: het tonen van de accountinfo van de gebruiker, de uitlogknop*

### Test 1

**Instructie:**
De gebruiker logt correct in met gebruikersnaam en wachtwoord en vervolgens met de juiste kleurcode op de Arduino.

**Verwacht resultaat:**
De gebruikerspagina wordt getoond met een welkomsboodschap. Hier staat de bijbehorende accountinfo vermeld.(?)

**Daadwerkelijk resultaat:**
...

### Test 2

**Instructie:**
De gebruiker logt correct in zoals Test 1.
De gebruiker navigeert op hun gebruikerspagina naar de knop 'Uitloggen' en klikt hier op.

**Verwacht resultaat:**
De inlogpagina voor gebruikersnaam en wachtwoord wordt getoond met lege velden.

**Daadwerkelijk resultaat:**
...



## Beheerpagina
*Hiermee testen we de requirements van: het tonen van de accountinfo van de beheerder, de uitlogknop, het tonen van de geregistreerde gebruikers, het toevoegen/verwijderen van gebruikers*


### Test 1

**Instructie:**
De beheerder logt correct in met gebruikersnaam en wachtwoord en vervolgens met de juiste kleurcode op de Arduino.

**Verwacht resultaat:**
De beheerpagina wordt getoond met een welkomsboodschap. 
Hier staat de accountinfo van de beheerder en worden beheerdersknoppen getoond om accounts te beheren ('Toon gebruikers', 'Gebruiker toevoegen', 'Gebruiker verwijderen')

**Daadwerkelijk resultaat:**
...


### Test 2

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Toon gebruikers'.

**Verwacht resultaat:**
Er wordt een lijst met geregistreerde gebruikers getoond.

**Daadwerkelijk resultaat:**
...


### Test 3

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker toevoegen'.

**Verwacht resultaat:**
Er worden een aantal velden getoond om een gebruiker toe te voegen aan de database ('e-mail adres', 'wachtwoord')

**Daadwerkelijk resultaat:**
...


### Test 4

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker toevoegen' en vult bij 'e-mail adres' *2fa@fontys.nl* in en bij 'wachtwoord' *testwachtwoord* in. Hierna klikt de beheerder op 'opslaan' en klikt daarna op de 'Toon gebruikers' knop.

**Verwacht resultaat:**
In de lijst met geregistreerde gebruikers staat 2fa@fontys.nl er nu ook tussen.

**Daadwerkelijk resultaat:**
...


### Test 5

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker toevoegen' en vult bij 'e-mail adres' *2fa@fontys.nl* in maar laat het veld 'wachtwoord' leeg. Hierna klikt de beheerder op 'opslaan'.

**Verwacht resultaat:**
Er komt een foutmelding in beeld 'Vul een geldig e-mail adres en/of wachtwoord in'

**Daadwerkelijk resultaat:**
...


### Test 6

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker toevoegen' en laat het veld 'e-mail adres' leeg maar vult in het veld 'wachtwoord' *testwachtwoord* in. Hierna klikt de beheerder op 'opslaan'.

**Verwacht resultaat:**
Er komt een foutmelding in beeld 'Vul een geldig e-mail adres en/of wachtwoord in'

**Daadwerkelijk resultaat:**
...


### Test 7

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker verwijderen'.

**Verwacht resultaat:**
Er wordt een zelfde lijst als bij Test 2 getoond. Hier kan de beheerder een of meerdere gebruikers selecteren om te verwijderen.

**Daadwerkelijk resultaat:**
...


### Test 8

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder klikt op 'Gebruiker verwijderen' en selecteert gebruiker *2fa@fontys.nl* Hierna klikt de beheerder op 'verwijderen' en klikt daarna op de 'Toon gebruikers' knop.

**Verwacht resultaat:**
In de lijst met geregistreerde gebruikers staat 2fa@fontys.nl er nu niet meer tussen.

**Daadwerkelijk resultaat:**
...



### Test 9 

**Instructie:**
De beheerder logt correct in zoals Test 1. 
De beheerder navigeert op hun gebruikerspagina naar de knop 'Uitloggen' en klikt hier op.

**Verwacht resultaat:**
De inlogpagina voor gebruikersnaam en wachtwoord wordt getoond met lege velden.

**Daadwerkelijk resultaat:**
...



