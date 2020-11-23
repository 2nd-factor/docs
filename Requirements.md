# Requirements Second Factor

# Milestone 2

## Functional requirements

### Website

# Frontend (Website - inlogpagina)

- De inlogpagina dient twee invulvelden te hebben voor het gebruikersnaam en het wachtwoord, zodat de gebruiker zijn/haar gebruikersgegevens in kan voeren.
- De inlogpagina moet een knop 'Inloggen' tonen waarmee de gebruiker na het invoeren van zijn/haar gegevens, de ingevoerde gegevens kan verzenden naar de backend. (Als de gegevens verzonden zijn, worden de invulvelden geleegd).
- De inlogpagina dient de boodschap "Incorrecte gebruikersnaam of wachtwoord" te tonen wanneer de door de gebruiker ingevoerde gegevens niet overeenkomen met de gegevens in de backend en vervolgens de gebruiker de kans te geven om alsnog de correcte gegevens in te voeren.
- De inlogpagina dient de gebruiker na het uitvoeren van een succesvolle inlog-procedure een tweede scherm te tonen waar een door de backend gegenereerde kleurencode wordt getoond.
- De door de backend gegenereerde kleurencode dient maximaal 30 seconden op de frontend te zien te zijn. Dit wordt bijgehouden door een timer die terug zal tellen van 30 naar 0. Daarna dient er maximaal 30 seconden lang een nieuwe kleurencode getoond te worden als de gebruiker geen kleurencode heeft ingevoerd.
- De frontend dient nadat de gebruiker de door de backend genereerde kleurencode heeft ingevoerd op de Arduino, en deze door de backend is goed bevonden, via de pagina met de gegenereerde kleurencode de gebruiker toegang te verschaffen tot de website. En de gebruiker een pagina te tonen met de informatie waar de gebruiker in kwestie recht op heeft.
- De frontend dient een normale gebruiker na het afronden van een succesvolle tweestaps-authenticatie procedure, een pagina voor normale gebruikers te tonen. (normale gebruiker content)
- De frontend dient een gebruiker met beheerder status na het afronden van een succesvolle tweestaps-authenticatie procedure, een pagina voor gebruikers met beheerder status te tonen. (beheerder content)
- De frontend dient de inlogpagina te tonen zodra een gebruiker die niet is ingelogd een beheerder of gebruiker pagina probeert te benaderen.

# Frontend (Website – normale gebruikerpagina)

- De normale gebruikerpagina dient een welkomstboodschap te tonen. Zodat de gebruiker weet dat hij/zij is ingelogd.
- De normale gebruikerpagina dient enkel informatie te tonen waar normale gebruikers recht op hebben.
- De normale gebruikerpagina dient een knop 'Uitloggen' te bevatten, zodat de ingelogde gebruiker de mogelijkheid heeft om uit te loggen.
- Wanneer de gebruiker op de knop ‘Uitloggen’ heeft geklikt, wordt de sessie afgebroken en wordt het beginscherm (inlogpagina) getoond, zodat hij/zij weet dat hij/zij is uitgelogd.

# Frontend (Website - beheerderpagina)

- De beheerderpagina dient een welkomstboodschap te tonen. Zodat de gebruiker met beheerder status weet dat hij/zij is ingelogd.
- De beheerderpagina dient een knop ‘Uitloggen’ te bevatten, zodat de ingelogde gebruiker met beheerder status de mogelijkheid heeft om uit te loggen.
- Wanneer de gebruiker met beheerder status op de knop ‘Uitloggen’ heeft geklikt, wordt de sessie afgebroken en wordt het beginscherm (inlogpagina) getoond, zodat hij/zij weet dat hij/zij is uitgelogd.
- De beheerderpagina moet invulvelden bevatten zodat de gebruiker met beheerder status de mogelijkheid heeft om gegevens van gebruikers in te voeren.
- De beheerderpagina moet een knop ‘Gebruiker toevoegen’ tonen waarmee de gebruiker met beheerder status de door de gebruiker met beheerder status ingevoerde gebruikersgegevens kan verzenden naar de backend, waar deze gegevens in de database worden geplaatst.
- De beheerderpagina moet een knop ‘Toon gebruikers’ tonen waarmee de gebruiker met beheerder status de gebruikersgegevens uit de database kan ophalen. Deze gegevens dienen getoond te worden in een lijst op de beheerderpagina.
- De beheerderpagina moet een knop ‘Gebruiker verwijderen’ tonen zodat de gebruiker met beheerder status de mogelijkheid heeft gebruikers te verwijderen uit de database.

### Backend

- De backend dient een database te hebben waarin gegevens gerelateerd aan gebruikers kunnen worden opgeslagen, zodat de backend deze gegevens vervolgens ook weer kan ophalen ter verificatie of verwijderen.
- In het geval dat er een nieuwe gebruiker wordt toegevoegd, dient de backend de ingevoerde gegevens te valideren, een gebruikersnaam moet met een hoofdletter beginnen en minimaal 2 letters bevatten. Een wachtwoord dient minimaal 6 tekens te bevatten, een hoofdletter, een cijfer en een speciaal teken.
- De backend dient de door de gebruiker ingevoerde gegevens te verifiëren met de gegevens in database. Als de gegevens niet overeenkomen, dient de backend de boodschap "Incorrecte gebruikersnaam of wachtwoord" naar de frontend te sturen, waar deze wordt getoond.
- Nadat de door de gebruiker ingevoerde gegevens zijn geverifieërd door de backend met de gegevens in de database en deze zijn goed bevonden, zal de backend een kleurencode genereren die maximaal uit 4 verschillende kleuren kan bestaan. Deze kleurencode zal random gegenereerd worden in een reeks van 4. Het is mogelijk dat een kleur meerdere malen voorkomt in de reeks. Deze kleurencode zal naar de frontend gestuurd worden, waar deze wordt getoond.
- De backend moet de gegenereerde kleurencode aan de gebruiker koppelen die zojuist het de inlog-procedure succesvol heeft afgerond via de frontend en deze opslaan in de database zodat de backend de met de Arduino ingevoerde kleurencode kan verifiëren met die in de database. Als de desbetreffende gebruiker de kleurencode correct in heeft gevoerd, moet de backend controleren welke rechten de gebruiker heeft. De backend stuurt een bericht naar de frontend met in de header de bevoegdheid van de gebruiker, zodat de juiste informatie op de frontend wordt getoond.
- De backend stuurt na een succesvolle inlog-procedure via de frontend de gegenereerde kleurencode naar de frontend en logt een tijdstip. Vanaf dat tijdstip zal de kleurencode 30 seconden zichtbaar zijn op de frontend zodat de gebruiker deze kan invoeren met de Arduino.
- De backend moet bij kunnen houden hoeveel tijd er nog rest voor de backend een nieuwe kleurencode moet genereren. Dit dient getoond te worden middels een timer op de frontend.
- De backend moet een nieuwe kleurencode genereren als de 30 seconden verstreken zijn en de backend heeft geen kleurencode via de Arduino ontvangen. De oudere kleurencode dient overschreven te worden.
- De backend dient nieuwe kleurencodes te genereren en naar de frontend te sturen zolang er geen kleurencode is ingevoerd met de Arduino die overeenkomt met de kleurencode in de database.
- De berichten afkomstig van de Arduino moeten worden voorzien van een timestamp, zodat met behulp van de timstamp van de door de backend gegenereerde kleurencode kan worden bepaald of de invoer van de Arduino binnen de 30 seconden valt.

### Arduino

- Arduino maakt en behoudt een verbinding met de backend
- Zolang er connectie is met de backend zal er een led lampje branden.
- De gebruiker kan doormiddel van meerdere knoppen een kleurcombinaties opstellen in de Arduino
- De gebruiker kan de ingevoerde kleurcombinaties versturen met een verzend-knop.
- De gebruiker kan de ingevoerde kleurcombinaties wissen met een reset-knop.

## Non-Funtional requirements

### Website

- Gebruikers moeten het wachtwoord wijzigen na het eerste keer inloggen
- De website moet mobile vriendelijk zijn

### Backend

- De backend moet verschillende gebruikers gelijktijdig kunnen afhandelen
- De kleurencode wordt na 30 seconden gereset
- De backend moet met meerdere Arduinos kunnen verbinden en de verschillende berichten kunnen afhandelen
- Na 10 foute inlogpogingen wordt het account geblokkeerd

### Arduino

- Indien er een fout optreed bij de Arduino, dan wordt dit aan de gebruiker gemeld(lampje)
