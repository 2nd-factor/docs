## Context analyse

# Beschrijving ontwerp

Dit project bestaat uit 3 verschillende onderdelen waarbij middels een arduino een 2FA (two-factor authentication) wordt uitgevoerd die op basis van kleurcombinaties werkt. De drie verschillende systemen zijn als volgt:

- Website
- Backend
- Arduino

De website dient als grafisch interface voor de authenticatie. Op de website kan eerst middels een gebruikersnaam en wachtwoord worden ingelogd, waarna er op de backend een kleurcombinatie wordt gegenereerd. 
Indien deze kleurcombinatie juist in de Arduino is ingevuld, dan is de 2FA geslaagd. Zowel de website als de Arduino maken middels een TCP protocol verbinding met de backend. De database wordt gebruikt voor het opslaan van gebruikersbestanden, Arduino codes en login-data.
