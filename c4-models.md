The following document explains the structure of our codebase.
The c4 model is a way of describing the architecture of a software project in mutliple levels of detail.
Layers of the c4 model are build on a certain layer of abstraction.
The next layer in the chain is supposed to give more information to the abstracted part of the diagram.

<details>
  <summary><b>C1 diagram</b></summary>
  
  ![alt text](/c4-diagrams/C1%20-%20System%20context%20diagram.svg "C1")
</details>
<details>
  <summary><b>C2 diagram</b></summary>  
	Het systeem bestaat uit een drietal containers.
	Als eerste heb je de Frontend-Server container waar de website opdraait.
	Als tweede heb je de Hardware container waar de Arduino (2nd-factor module) in staat.
	Als Derde is er de Server. Deze container bevat zowel de database, API en een developer view module.
	Vanuit de website kun je een request sturen naar de Server. In de Server zal het API component het communiceren op zich nemen 
	en daarbij de berichten repository bijhouden. In de Server container zal een Swagger module komen die het uittesten 
	en bekijken van de API beschrijving faciliteert.
	De 2nd-factor module zal bestaan uit een Arduino met verschillende componenten en Wi-Fi mogelijkheid. 
	Deze module zal via TCP communiceren met de Server.
  
  ![alt text](/c4-diagrams/C2%20-%20Container%20diagramv2.svg "C2")

</details>
<details>
  <summary><b>C3 diagram</b></summary>

In het component level digram worden de hardware container en de Server verder toegelicht. Hierbij wordt dieper ingegaan op de verschillende components die zich bevinden in deze twee containers.

De backend server heeft een tweetal controllers die de http requests opvangen en verder afhandelen. Verder zit er nog een developer component die de toegang van de developer bewerkstelligt. De GenerateCode controller laat via de Generate Code component de 2fa-code genereren. De VerifyCode controller bewerkstelligt dat met de Code verifier component.
De verschillende opgevraagde codes worden opgeslagen in een database component.
De code handler component heeft verbinding met de hardware container en registreert inkomende signalen en slaat deze op in de database.

De hardware module heeft een aantal controllers en handlers. De Communicatie met de backend gebeurt via de _communicationHandler_. De Wifi verbinding wordt gedaan door de WifiConnectionHandler component. Deze maakt en behoud de verbinding. De ButtonHandler behandeld alle analoge en digitale(PWM) in en outputs.

![alt text](/c4-diagrams/C3%20-%20Component%20diagram.svg "C3")

</details>
