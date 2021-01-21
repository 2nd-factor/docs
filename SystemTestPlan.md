# System Test

# Second Factor

# Milestone 2

#

## System testing op interactie met Arduino
_Hiermee testen we de requirements van: Er wordt een een bevestiging van actieve verbinding getoond, er is een manier om een kleurencode in te geven, te versturen en te wissen.

### Test 1

**Instructie:**
Sluit de Arduino aan wanneer de server actief is. 

**Verwacht resultaat:**
Zodra de Arduino aan staat, gaat het ledje branden ter bevestiging van een actieve verbinding. 

**Daadwerkelijk resultaat:**
Het ledje brandt zodra er een actieve verbinding aanwezig is. Deze komt tot stand zodra de 'verstuur'-knop op de Arduino wordt ingedrukt.


### Test 2

**Instructie:**
Schakel de Arduino in wanneer de server inactief is.

**Verwacht resultaat:**
Zodra de Arduino aan staat, blijft het ledje uit ter bevestiging dat er geen actieve verbinding is. 

**Daadwerkelijk resultaat:**
Na indrukken 'verstuur'-knop, blijft het ledje 30 seconden uit en knippert daarna vier keer om aan te geven dat er geen actieve verbinding is.


### Test 3

**Instructie:**
Druk drie keer de 'blauwe' knop in. 

**Verwacht resultaat:**
Er gaan drie blauwe (RGB)-leds branden.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.



### Test 4

**Instructie:**
Druk drie keer de 'rode' knop in.

**Verwacht resultaat:**
Er gaan drie rode (RGB)-leds branden.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.


### Test 5

**Instructie:**
Druk drie keer de 'groene' knop in.


**Verwacht resultaat:**
Er gaan drie groene (RGB)-leds branden.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.


### Test 6

**Instructie:**
Druk de 'groene', 'rode', en 'blauwe' knoppen ieder 1x in op de Arduino.

**Verwacht resultaat:**
Er gaan op de Arduino een groene, een rode en een blauwe (RGB)-led branden.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.

### Test 7

**Instructie:**
Druk drie keer op de 'groene' knop op de Arduino.
Druk hierna op de reset knop en druk drie keer op de 'rode' knop. 

**Verwacht resultaat:**
Na het invullen van de eerste reeks, worden de (RGB)-leds groen. Na het indrukken van de reset-knop gaan de (RGB)-leds allemaal uit en na de tweede reeks, worden de (RGB)-leds rood.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.


## User acceptance tests op front-end
_Hiermee testen we de requirements van: Er is een 'genereer code'-knop op de frontend, wanneer deze ingedrukt wordt, toont de frontend een kleurencode van 3 (verschillende) kleuren.

### Test 1

**Instructie:**
Klik op de website knop 'genereer code'. 

**Verwacht resultaat:**
De 'genereer code'-knop wordt vervangen door de 'verifieer'-knop.
Er verschijnt een kleurencode van 3 (verschillende) kleuren. 
Er komt tegelijk met de kleurencode een timer in beeld die de geldige 30 seconden aftelt.


**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.

### Test 2

**Instructie:**
Klik op de knop 'genereer code' en wacht 30 seconden zonder iets in te voeren.

**Verwacht resultaat:**
De 'genereer code'-knop wordt vervangen door de 'verifieer'-knop.
Er verschijnt een kleurencode van 3 (verschillende) kleuren.  
Er komt tegelijk met de kleurencode een timer in beeld die de geldige 30 seconden aftelt.
Nadat de timer 0 seconden heeft bereikt, komt de 'genereer-code'-knop weer in beeld. Zowel de 'verifieer'-knop en de vervallen code verdwijnen van de webpagina.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.


### Test 3
**Instructie:**
Klik op de knop 'genereer code', lees de kleurencode en vul deze in op de Arduino. 
Druk op de verzendknop van de Arduino en op de 'verifieer'-knop op de website. 

**Verwacht resultaat:**
Je ziet een 'succes' bericht op de website.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.

### Test 4
**Instructie:**
Klik op de knop 'genereer code', lees de kleurencode maar vul een andere code in op de Arduino.  
Druk op de verzendknop van de Arduino en op de 'verifieer'-knop op de website.  

**Verwacht resultaat:**
Je ziet een 'fout' bericht op de website.

**Daadwerkelijk resultaat:**
Zoals verwacht resultaat.


