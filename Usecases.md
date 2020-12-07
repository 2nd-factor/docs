# Usecases

## Usecase inloggen

- Naam : Inloggen
- Doel : Gebruiker laten inloggen middels een 2FA
- Actoren : Gebruiker
- Aannames : De gebruiker heeft een code aangevraagd.
- Beschrijving: De gebruiker gaat inloggen d.m.v. 2FA door op de website een code aan te vragen en vervolgens op de arduino deze code in te vullen.
                Om vervolgens vanuit de website te controleren of de ingevulde code juist ingevuld is.
- Uitzondering:
- Resultaat : De gebruiker krijgt een bevestiging dat de code correct is ingevuld.

### User story

Als gebruiker wil ik middels een 2FA systeem veilig kunnen inloggen

## Usecase verificatie

- Naam : verificatie
- Doel : Het systeem controleert of de ingevulde code matched met de verwachte code.
- Actoren : Systeem
- Aannames : De gebruiker heeft de code goed ontvangen en heeft deze vervolgens correct op de arduino ingevuld.
- Beschrijving: Het systeem controleert of de ontvangen code overeenkomt met de verzonde gegenereerde code.
- Uitzondering:
- Resultaat : De code is succesvol vergeleken en geaccepteerd als valide code.

### User story

Ik wil dat het systeem controleert of de code die ik heb ingevuld correct is.

## Usecase Code aanvragen

- Naam : code aanvragen
- Doel : Op de website vraagt de gebruiker om een code deze wordt bij aankomst op de website getoond.
- Actoren : Gebruiker
- Aannames :
- Beschrijving: De gebruiker vraagt d.m.v. een knop een code aan. Deze wordt op de server gegenereerd (random) en laten zien op de website.
- Uitzondering:
- Resultaat : Er wordt een random gegenereerde code laten zien aan de gebruiker.

### User story

Ik wil dat ik iedere keer als ik een code aanvraag een nieuwe random code wordt gegenereerd.
