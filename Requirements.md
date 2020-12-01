# Requirements Second Factor

# Milestone 2

## Functional requirements

### Website

# Frontend (Website)

- De website heeft een knop 'genereer code'.
- Na het klikken op de 'genereer code'-knop zal een tweede scherm laden, waar een door de backend gegenereerde kleurencode wordt getoond.
- De door de backend gegenereerde kleurencode dient maximaal 30 seconden op de frontend te zien te zijn. Dit wordt bijgehouden door een timer die terug zal tellen van 30 naar 0. 
- Als de juiste code niet binnen 30 seconden wordt ingevoerd, dan verschijnt de 'genereer code'-knop weer in beeld.

- De frontend dient nadat de gebruiker de door de backend genereerde kleurencode heeft ingevoerd op de Arduino, en deze door de backend is goed bevonden, via de pagina met de gegenereerde kleurencode een succes bericht te tonen.




### Backend

- Nadat de gebruiker in de front-end de genereer knop drukt zal de backend een cijferreeks genereren die maximaal uit 3 verschillende cijfers kan bestaan. Met de keuze 1,2 of 3. Deze cijfercode zal random gegenereerd worden. Het is mogelijk dat een cijfer meerdere malen voorkomt in de reeks. Deze cijfercode zal opgeslage worden in de database en  naar de frontend gestuurd worden, waar deze wordt vertaald naar kleurcombinatie.
- De backend controleert of de gegenereerde cijfercode overeenkomt met de ingevoerde combinatie vanuit de Arduino en stuurt een uitkomst naar de frontend.
- De backend stuurt de gegenereerde cijfercode naar de frontend en logt een timestamp. Vanaf dat tijdstip zal de cijfercode 30 seconden zichtbaar zijn op de frontend zodat de gebruiker deze kan invoeren met de Arduino.
- De backend moet een nieuwe cijfercode genereren als de 30 seconden verstreken zijn en de backend heeft geen cijfercode via de Arduino ontvangen. De oudere cijfercode dient overschreven te worden in de database.
- De berichten afkomstig van de Arduino moeten worden voorzien van een timestamp door de backend, de backend kan de timestamp van het Arduino bericht vergelijken met de timestamp van de aangemaakte cijferreeks vanuit de backend. Hiermee wordt bepaald of deze binnen 30 seconden is ontvangen.


### Arduino

- Arduino maakt en behoudt een verbinding met de backend
- Zolang er connectie is met de backend zal er een led lampje branden.
- De gebruiker kan doormiddel van meerdere knoppen een kleurcombinaties opstellen in de Arduino
- De gebruiker kan de ingevoerde kleurcombinaties versturen met een verzend-knop.
- De gebruiker kan de ingevoerde kleurcombinaties wissen met een reset-knop.

## Non-Funtional requirements


### Backend

- De kleurencode wordt na 30 seconden gereset
- De backend moet met meerdere Arduinos kunnen verbinden en de verschillende berichten kunnen afhandelen
