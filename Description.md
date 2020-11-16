## Contaxt analyse

# Beschrijving ontwerp

Dit project bestaat uit 3 verschillende onderdelen waarbij middels een arduino een 2FA wordt uitgevoerd die op basis van kleurcombinaties werkt. De drie verschillende systemen zijn als volgt:

- Website
- Backend
- Arduino

De website dient als grafisch interface voor de authenticatie. Op de website kan eerst middels een gebruikersnaam en wachtwoord worden ingelogd, waarna er op de backend een kleurcombinatie wordt gegenereerd. Indien deze kleurcombinatie juist in de arduino is ingevuld, dan is de 2FA geslaagd. Zowel de website als de arduino maken middels een TCP protocol verbinding met de backend. De database wordt gebruikt voor het oplsaan van gebruikersbestanden, arduino codes en logindata.
