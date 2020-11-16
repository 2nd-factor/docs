# Frontend (Website - inlogpagina)   

- De inlogpagina dient twee invulvelden te hebben voor de gebruikersnaam en het gebruikerswachtwoord, zodat de gebruiker zijn/haar gebruikersgegevens in  kan voeren.
- De inlogpagina moet een knop 'Inloggen' tonen waarmee de gebruiker na het invoeren van zijn/haar gegevens, de ingevoerde gegevens kan verzenden naar de backend. (Als de gegevens verzonden zijn, worden de invulvelden geleegd).
- De inlogpagina dient een foutmelding te tonen wanneer de door de gebruiker ingevoerde gegevens niet overeenkomen met de gegevens in de backend.
- De inlogpagina dient een boodschap "Something went wrong, try again" te tonen wanneer de door de gebruiker ingevoerde gegevens niet overeenkomen met de gegevens in de backend en vervolgens de gebruiker de kans te geven om alsnog de correcte gegevens in te voeren.
- De inlogpagina dient de gebruiker na het uitvoeren van een succesvolle inlog-procedure een tweede scherm te tonen waar een door de backend gegenereerde kleurencode wordt getoond.
- De frontend dient nadat de gebruiker de door de backend genereerde kleurencode heeft ingevoerd op de Arduino, en deze door de backend is goed bevonden, via de pagina met de gegenereerde kleurencode de gebruiker toegang te verschaffen tot de website. En de gebruiker een pagina te tonen met de informatie waar de gebruiker in kwestie recht op heeft.
- De frontend dient een normale gebruiker na het afronden van een succesvolle tweestaps-authenticatie procedure, een pagina voor normale gebruikers te tonen. (normale gebruiker content)
- De frontend dient een gebruiker met beheerder status na het afronden van een succesvolle tweestaps-authenticatie procedure, een pagina voor gebruikers met beheerder status te tonen. (beheerder content)
- De frontend dient een foutmelding te tonen zodra een gebruiker die niet is ingelogd als gebruiker met beheerder status de beheerder pagina probeert te benaderen. 

# Frontend (Website – normale gebruikerpagina)   

- De normale gebruikerpagina dient de boodschap “Hallo + gebruikersnaam” te tonen. Zodat de gebruiker weet dat hij/zij is ingelogd.
- De normale gebruikerpagina dient enkel informatie te tonen waar normale gebruikers recht op hebben.
- De normale gebruikerpagina dient een knop ‘Uitloggen’ te bevatten, zodat de ingelogde gebruiker de mogelijkheid heeft om uit te loggen.
- Wanneer de gebruiker op de knop ‘Uitloggen’ heeft geklikt, wordt de sessie afgebroken en wordt het beginscherm (inlogpagina) getoond, zodat hij/zij weet dat hij/zij is uitgelogd.

# Frontend (Website - beheerderpagina)   

- De beheerderpagina dient de boodschap “Hallo + gebruikersnaam” te tonen. Zodat de gebruiker met beheerder status weet dat hij/zij is ingelogd.
- De beheerderpagina dient een knop ‘Uitloggen’ te bevatten, zodat de ingelogde gebruiker met beheerder status de mogelijkheid heeft om uit te loggen.
- Wanneer de gebruiker met beheerder status op de knop ‘Uitloggen’ heeft geklikt, wordt de sessie afgebroken en wordt het beginscherm (inlogpagina) getoond, zodat hij/zij weet dat hij/zij is uitgelogd.
- De beheerderpagina moet invulvelden bevatten zodat de gebruiker met beheerder status de mogelijkheid heeft om gegevens van gebruikers in te voeren.
- De beheerderpagina moet een knop ‘Gebruiker toevoegen’ tonen waarmee de gebruiker met beheerder status de door de gebruiker met beheerder status ingevoerde gebruikersgegevens kan verzenden naar de backend, waar deze gegevens in de database worden geplaatst.
- De beheerderpagina moet een knop ‘toon gebruikers’ tonen waarmee de gebruiker met beheerder status de gebruikersgegevens uit de database kan ophalen. Deze gegevens dienen getoond te worden in een lijst op de beheerderpagina.
- De beheerderpagina moet een knop ‘Gebruiker verwijderen’ tonen zodat de gebruiker met beheerder status de mogelijkheid heeft gebruikers te verwijderen uit de database.
