# User Acceptance Test

# Second Factor

# Milestone 2

## Login met gebruikersnaam en wachtwoord

_Hiermee testen we de requirements van: in te vullen velden bij 'e-mailadres' en 'wachtwoord', het verzenden van inloggegevens met een 'Inloggen' knop, het tonen van een boodschap bij invoer van foutieve gegevens (op diverse manieren), het tonen van een kleurencode bij correcte login_

### Test 1

**Instructie:**
De gebruiker vult een correct e-mailadres en wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een kleurencode te zien die hij/zij dient in te voeren op de Arduino.

**Daadwerkelijk resultaat:**
...

### Test 2

**Instructie:**
De beheerder vult een correct e-mailadres en wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De beheerder krijgt een kleurencode te zien die hij/zij dient in te voeren op de Arduino.

**Daadwerkelijk resultaat:**
...

### Test 3

**Instructie:**
De gebruiker vult een incorrect e-mailadres en een correct wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 4

**Instructie:**
De beheerder vult een incorrect e-mailadres en wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De beheerder krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 5

**Instructie:**
De gebruiker vult een correct e-mailadres en een incorrect wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 6

**Instructie:**
De beheerder vult een correct e-mailadres en een incorrect wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De beheerder krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 7

**Instructie:**
De gebruiker vult een incorrect e-mailadres en een correct wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 8

**Instructie:**
De beheerder vult een incorrect e-mailadres en een correct wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 9

**Instructie:**
De gebruiker of beheerder vult alleen een e-mailadres in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

### Test 10

**Instructie:**
De gebruiker of beheerder vult alleen een wachtwoord in, klikt vervolgens op de 'Inloggen' knop.

**Verwacht resultaat:**
De gebruiker krijgt een melding te zien "Incorrect e-mailadres of wachtwoord".

**Daadwerkelijk resultaat:**
...

## Kleuren verificatie na succesvolle inlog-procedure met gebruiker info

_Hiermee testen we de requirements van: een kleurencode die maximaal 30 seconden geldig is, de welkomstboodschap op gebruikers- en beheerderspagina's, verificatie van kleurencode in de backend, het invoeren van de kleurencode op de Arduino, gebruik van de knoppen op de Arduino (kleuren, verzendknop, resetknop)._

### Test 1

**Instructie:**
De gebruiker of beheerder vult het correcte e-mailadres en wachtwoord in, klikt vervolgens op de 'Inloggen' knop. Ze wachten 30 seconden zonder iets in te vullen op de Arduino.

**Verwacht resultaat:**
De website ververst en toont een nieuw gegenereerde kleurencode.

**Daadwerkelijk resultaat:**
...

### Test 2

**Instructie:**
De gebruiker vult na inloggen de getoonde kleuren correct in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont de gebruikerspagina met een welkomstboodschap.

**Daadwerkelijk resultaat:**
...

## Test 3

**Instructie:**
De beheerder vult na inloggen de getoonde kleuren correct in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont de beheerderspagina met een welkomstboodschap.

**Daadwerkelijk resultaat:**
...

### Test 4

**Instructie:**
De gebruiker vult de getoonde kleuren verkeerd in op de Arduino en drukt op de verzendknop.

**Verwacht resultaat:**
De website toont een foutmelding 'Verkeerde kleurencode' en toont een nieuw gegenereerde kleurencode.

**Daadwerkelijk resultaat:**
...

### Test 5

**Instructie:**
De gebruiker vult de getoonde kleuren verkeerd in op de Arduino, drukt op de resetknop en vult daarna de juiste kleurencode in.
Hierna drukt de gebruiker op de verzendknop.

**Verwacht resultaat:**
De website toont de gebruikerspagina met een welkomstboodschap.

**Daadwerkelijk resultaat:**
...

## Gebruikerspagina

_Hiermee testen we de requirements van: het tonen van de accountinfo van de gebruiker, de 'Uitloggen' knop_

### Test 1

**Instructie:**
De gebruiker logt correct in met e-mailadres en wachtwoord en vervolgens met de juiste kleurencode op de Arduino.

**Verwacht resultaat:**
De gebruikerspagina wordt getoond met een welkomstboodschap. Hier staat de bijbehorende accountinfo vermeld.(?)

**Daadwerkelijk resultaat:**
...

### Test 2

**Instructie:**
De gebruiker logt correct in zoals Test 1.
De gebruiker navigeert op hun gebruikerspagina naar de knop 'Uitloggen' en klikt hier op.

**Verwacht resultaat:**
De inlogpagina voor e-mailadres en wachtwoord wordt getoond met lege velden.

**Daadwerkelijk resultaat:**
...

## Beheerpagina

_Hiermee testen we de requirements van: het tonen van de accountinfo van de beheerder, de 'Uitloggen' knop, het tonen van de geregistreerde gebruikers, het toevoegen/verwijderen van gebruikers_

### Test 1

**Instructie:**
De beheerder logt correct in met e-mailadres en wachtwoord en vervolgens met de juiste kleurencode op de Arduino.

**Verwacht resultaat:**
De beheerpagina wordt getoond met een welkomstboodschap.
Hier staat de accountinfo van de beheerder en worden beheerdersknoppen getoond om accounts te beheren ('Toon gebruikers', 'Gebruiker toevoegen', 'Gebruiker verwijderen', 'Opslaan')

**Daadwerkelijk resultaat:**
...

### Test 2

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Toon gebruikers' knop.

**Verwacht resultaat:**
Er wordt een lijst met geregistreerde gebruikers getoond.

**Daadwerkelijk resultaat:**
...

### Test 3

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker toevoegen' knop.

**Verwacht resultaat:**
Er worden een aantal velden getoond om een gebruiker toe te voegen aan de database ('e-mailadres', 'wachtwoord')

**Daadwerkelijk resultaat:**
...

### Test 4

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker toevoegen' knop en vult bij 'e-mailadres' *2fa@fontys.nl* in en bij 'wachtwoord' _testwachtwoord_ in. Hierna klikt de beheerder op de 'Opslaan' knop en klikt daarna op de 'Toon gebruikers' knop.

**Verwacht resultaat:**
In de lijst met geregistreerde gebruikers staat 2fa@fontys.nl er nu ook tussen.

**Daadwerkelijk resultaat:**
...

### Test 5

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker toevoegen' knop en vult bij 'e-mailadres' *2fa@fontys.nl* in maar laat het veld 'wachtwoord' leeg. Hierna klikt de beheerder op de 'Opslaan' knop.

**Verwacht resultaat:**
Er komt een foutmelding in beeld 'Vul een geldig e-mailadres en/of wachtwoord in'

**Daadwerkelijk resultaat:**
...

### Test 6

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker toevoegen' knop en laat het veld 'e-mailadres' leeg maar vult in het veld 'wachtwoord' _testwachtwoord_ in. Hierna klikt de beheerder op de 'opslaan' knop.

**Verwacht resultaat:**
Er komt een foutmelding in beeld 'Vul een geldig e-mailadres en/of wachtwoord in'

**Daadwerkelijk resultaat:**
...

### Test 7

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker verwijderen' knop.

**Verwacht resultaat:**
Er wordt een zelfde lijst als bij Test 2 getoond. Hier kan de beheerder een of meerdere gebruikers selecteren om te verwijderen.

**Daadwerkelijk resultaat:**
...

### Test 8

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder klikt op de 'Gebruiker verwijderen' knop en selecteert gebruiker *2fa@fontys.nl* Hierna klikt de beheerder op de 'verwijderen' knop en klikt daarna op de 'Toon gebruikers' knop.

**Verwacht resultaat:**
In de lijst met geregistreerde gebruikers staat 2fa@fontys.nl er nu niet meer tussen.

**Daadwerkelijk resultaat:**
...

### Test 9

**Instructie:**
De beheerder logt correct in zoals Test 1.
De beheerder navigeert op hun gebruikerspagina naar de knop 'Uitloggen' en klikt hier op.

**Verwacht resultaat:**
De inlogpagina voor emailadres en wachtwoord wordt getoond met lege velden.

**Daadwerkelijk resultaat:**
...
