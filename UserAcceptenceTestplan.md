# User Acceptance Test

# Second Factor

# Milestone 2

#

## User acceptance testen op interactie met 2FA
_Hiermee testen we de requirements van: Er wordt een een bevestiging van actieve verbinding getoond, er is een manier om een kleurencode in te geven, te versturen en te wissen.

### Test AD-power_01

**Instructie:**
De gebruiker plugt de Arduino in wanneer de server actief is. 

**Verwacht resultaat:**
Zodra de Arduino is ingeschakeld, wordt met een brandend ledje bevestigd dat er een actieve verbinding is. 

**Daadwerkelijk resultaat:**
...


### Test AD-power_00

**Instructie:**
De gebruiker schakelt de Arduino in wanneer de server inactief is.

**Verwacht resultaat:**
Zodra de Arduino is ingeschakeld, blijft het ledje uit om te bevestigen dat er geen actieve verbinding is. 

**Daadwerkelijk resultaat:**
...


### Test AD-colorBlue_00

**Instructie:**
De gebruiker vult drie keer de kleur blauw in bij de Arduino door het indrukken van de corresponderende knop. 

**Verwacht resultaat:**
Deze invoer wordt met drie blauwe, brandende (RGB)-leds bevestigd.

**Daadwerkelijk resultaat:**
...



### Test AD-colorRed_00

**Instructie:**
De gebruiker vult drie keer de kleur rood in bij de Arduino door het indrukken van de corresponderende knop. 

**Verwacht resultaat:**
Deze invoer wordt met drie rode, brandende (RGB)-leds bevestigd.

**Daadwerkelijk resultaat:**
...


### Test AD-colorGreen_00

**Instructie:**
De gebruiker vult drie keer de kleur groen in bij de Arduino door het indrukken van de corresponderende knop. 

**Verwacht resultaat:**
Deze invoer wordt met drie groen, brandende (RGB)-leds bevestigd.

**Daadwerkelijk resultaat:**
...


### Test AD-colorRGB00

**Instructie:**
De gebruiker vult de kleuren rood, groen en blauw ieder 1x in bij de Arduino door het indrukken van de corresponderende knoppen. 

**Verwacht resultaat:**
Deze invoer wordt met een rood, een groen en een blauwe brandende (RGB)-led bevestigd.

**Daadwerkelijk resultaat:**
...

### Test AD-reset_00

**Instructie:**
De gebruiker vult drie keer de kleur groen in bij de Arduino door het indrukken van de corresponderende knop. 
Hierna drukt de gebruiker op de reset knop en vult drie keer de kleur rood in bij de Arduino door het indrukken van de corresponderende knop. 

**Verwacht resultaat:**
Na het invullen van de eerste reeks, worden de (RGB)-leds groen. Na het indrukken van de reset-knop gaan de (RGB)-leds allemaal uit en na het invullen van de tweede reeks, worden de (RGB)-leds rood.

**Daadwerkelijk resultaat:**
...


## User acceptance tests op front-end
_Hiermee testen we de requirements van: Er is een 'genereer code'-knop op de frontend, wanneer deze ingedrukt wordt, toont de frontend een kleurencode van 3 (verschillende) kleuren.

### Test FE-generate_00

**Instructie:**
De gebruiker klikt op de knop 'genereer code'. 

**Verwacht resultaat:**
De 'genereer code'-knop verdwijnt van de pagina en wordt vervangen door de 'verifieer'-knop.
Daarbij wordt ook een kleurencode getoond van 3 (verschillende) kleuren. 
Er komt tegelijk met de kleurencode een timer in beeld die de geldige 30 seconden aftelt.


**Daadwerkelijk resultaat:**
...

### Test FE-generate_01

**Instructie:**
De gebruiker klikt op de knop 'genereer code' en wacht 30 seconden zonder iets in te voeren.

**Verwacht resultaat:**
De 'genereer code'-knop verdwijnt van de pagina en wordt vervangen door de 'verifieer'-knop.
Daarbij wordt ook een kleurencode getoond van 3 (verschillende) kleuren.  
Er komt tegelijk met de kleurencode een timer in beeld die de geldige 30 seconden aftelt.
Nadat de timer 0 seconden heeft bereikt, verschijnt de 'genereer-code'-knop weer in beeld en zowel de 'verifieer'-knop en de vervallen code verdwijnen van de pagina.

**Daadwerkelijk resultaat:**
...


### Test FE-genVer_00
**Instructie:**
De gebruiker klikt op de knop 'genereer code', leest de kleurencode van de pagina en vult deze in op de 2FA door middel van de corresponderende knoppen. 
Nadat de gebruiker de, op de website afgebeelde code heeft ingevoerd, drukt hij op de verzendknop op de 2FA.
Hierna drukt hij op de 'verifieer'-knop op de website. 

**Verwacht resultaat:**
Er verschijnt er een 'succes' bericht op de website.

**Daadwerkelijk resultaat:**
...

### Test FE-genVer_01
**Instructie:**
De gebruiker klikt op de knop 'genereer code', leest de kleurencode van de pagina en vult een andere code in op de 2FA door middel van de corresponderende knoppen. 
Nadat de gebruiker de, verkeerde code heeft ingevoerd, drukt hij op de verzendknop op de 2FA.
Hierna drukt hij op de 'verifieer'-knop op de website. 

**Verwacht resultaat:**
Er verschijnt er een 'fout' bericht op de website.

**Daadwerkelijk resultaat:**
...


