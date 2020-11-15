#Requirements Second Factor
#Milestone 2

##Front-end

**Must have**

* Er is een invulveld voor een gebruikersnaam.
* Er is een invulveld voor een wachtwoord.
* Er is een log-in button om de ingevulde velden te versturen.
* Na een correcte log-in wordt een TCP-connectie met de back-end gemaakt.
* Na een correcte log-in wordt de kleuren-combinatie vanuit de backend op de website getoond.
* Na een correct ingevulde kleurencombinatie op de Arduino, wordt een 'succes' scherm getoond. (?)

**Should have**

* Na een correcte log-in met admin-gegevens wordt een beheerderspagina getoond met extra informatie zoals ingelogde gebruikers, timestamps, etc.


##Back-end 

**Must have**

* Er wordt een socket-connectie opgezet naar de Arduino.
* Er wordt een TCP-connectie opgezet met de front-end.
* Er is een database waar gebruikers-gegevens worden opgeslagen.
* Er is een database die Arduino berichten opslaat met een timestamp.
* Er is een functie die ingevulde gebruikers-gegevens controleert op juistheid in de database.
* Er is een functie die op basis van een correcte log-in een willekeurige kleurencombinatie aanmaakt en naar de frontend verstuurt.
* De aangemaakte kleurencombinatie wordt in de database opgeslagen bij de gebruikersinfo. 
* Er is een functie die de input van de Arduino kan interpreteren en vergelijken met de opgeslagen velden in de database.

**Could have**

* Er kunnen combinaties van kleuren aan een log-in gekoppeld worden. 


##Arduino

**Must have**

* De Arduino maakt verbinding met de back-end.
* De gebruiker kan kleuren-input invoeren door op bijpassende knoppen te drukken.
* De gebruiker kan de ingevoerde kleuren-input versturen met een verzend knop.
* De gebruiker kan de ingevoerde kleuren-input wissen met een reset knop.

**Should have**

* De Arduino heeft een display die laat zien welke kleuren er door de gebruiker zijn ingevoerd.

**Could have**

* De gebruiker kan combinaties van kleuren invoeren.