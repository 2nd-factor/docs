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
	Er zijn 3 verschillende containers met ieder zijn eigen componenten.
	Als eerste heb je de Frontend-Server container waar de website opdraait.
	Als tweede heb je de Hardware container waar de Arduino (2nd-factor module) in staat.
	Als Derde is er de Server. Deze container bevat zowel de database, API en een developer view module.
	Vanuit de website kun je een request sturen naar de Server. In de Server zal het API component het communiceren op zich nemen 
	en daarbij de berichten repository bijhouden. In de Server container zal een Swagger module komen die het uittesten 
	en bekijken van de API beschrijving faciliteert.
	De 2nd-factor module zal bestaan uit een Arduino met verschillende componenten en Wi-Fi mogelijkheid. 
	Deze module zal via TCP communiceren met de Server.
  
  ![alt text](/c4-diagrams/C2%20-%20Container%20diagram.svg "C2")

</details>
<details>
  <summary><b>C2 diagram</b></summary> 
   Components

![alt text](/c4-diagrams/C3%20-%20Component%20diagram.svg "C3")

</details>
