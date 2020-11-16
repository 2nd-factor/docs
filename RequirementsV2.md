# Requirements Second Factor

# Milestone 2

## Functional requirements

### Website

- De website heeft een gebruikersnaamveld en een wachtwoord veld
- De website heeft een inlog knop die de gebruiker moet indrukken op de ingevoerde gegevens te valideren
- De website geeft een foutmelding als de gebruikersnaam of wachtwoord niet juist zijn
- Na het juist inloggen verschijnt een tweede scherm voor het valideren van de 2fa
- De website bevat een beheerderspagina waarop ingelogde personen zichtbaar zijn
- De beheerpagina kan gebruikers verwijderen en teovoegen

### Backend

- De backend valideert alle ingevoerde inloggegevens
- Na het inloggen wordt het tijdstip gelogd
- Voor het inloggen wordt een TCP connectie gebruikt
- De backend maakt tijdens het opstarten een TCP connectie met de arduino
- De backend heeft een database
- Berichten vanuit de arduino worden opgeslagen met een timestamp
- De backend genereert na het inloggen een 2fa kleurcombinatie en verstuurt deze naar de website
- De backend verifieert de aangemaakte kleurcombinatie met het bericht vanuit de arduino

### Arduino

- Arduino maakt en behoudt een tcp verbinding met de backend
- De gebruiker kan kleurcombinaties invoeren in de arduino
- De gebruiker kan de ingevoerde kleuren-input versturen met een verzend knop.
- De gebruiker kan de ingevoerde kleuren-input wissen met een reset knop.

## Non-Funtional requirements

### Website

- Gebruikers moeten het wachtwoord wijzigen na het eerste keer inloggen
- De website moet mobile vriendelijk zijn

### Backend

- De backend moet verschillende gebruikers gelijktijdig kunnen afhandelen
- De kleurcombinatie wordt na 30 seconden gereset
- De backend moet met meerdere arduinos kunnen verbinden en de verschillende berichten kunnen afhandelen
- Na 10 foute inlogpogingen wordt het account geblokkeerd

### Arduino

- Indien er een fout optreed bij de arduino dan wordt dit aan de gebruiker gemeld(lampje)
