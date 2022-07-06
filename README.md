Hey hoi, welkom. Als het goed is heb jij (of jullie) de opdracht gekregen om deze E-Learning af te maken als project voor je stage.

Wij hebben al een flinke basis gelegd voor dit programma, dus het is maar een kwestie van tijd voor dit programma volledig af is.

Helaas hebben wij flink verkeerd gepland waardoor het project niet af is. Ook hadden wij geen ervaring dus was het moeilijk opstarten voor ons.

Het project kan misschien eerst als chaos overkomen, maar ik hoop dat wij het zo duidelijk mogelijk hebben uitgelegd hier.

Als er vragen zijn, contact Bqnaan#7978 op discord. of mail naar sjoerdsteeman@gmail.com

#############################################################################

Het maken van de quiz,

Het maken van de quiz is vrij gemakkelijk. Er zijn hierbij 3 scripts die ik gebruik om de quiz functioneel te houden. 

Answerscript, QuestionsAndAnswers en quizmanager. Deze scripts zijn te vinden in Assets > Scripts > Quiz scripts.

Ik heb mijn best gedaan om de code hierin zo duidelijk mogelijk te commenten

##

Om een volledige quiz pagina te creëeren, is het mogelijk om te kopiëren van een bestaande quiz. Een fully functional quiz om hierbij te gebruiken is de quiz van Plugkranen.

Om hier te komen moet je naar Assets > Scenes > Infopaginas > Kleppen en kranen > Plugkranen gaan.

Wanneer je in de quiz pagina bent hiervan, druk je op het gameobject genaamd "quizmanager".

In inspector, druk op de dropdown genaamd "Qn A". Hierbij kan je vragen bewerken, toevoegen en verwijderen. Hetzelfde geldt voor de antwoorden.

#################################################################################

Het maken van een puzzel,

Voor het maken van een puzzel heb ik sprites van de onderdelen uit de schematische tekeningen gebruikt.
Elke sprite geef je het Draggable script en een polygon collider 2D.

Voor de plaatsen van de puzzelstukken gebruik je dezelfde sprite van het puzzelstuk.
Bij deze heb ik de kleur zwart gemaakt en de doorzichtigheid op 90 gezet.
Deze hoeven geen script en collider.

Om de puzzel volledig werkend te krijgen heb ik een GameObject toegevoegd met daarin het SnapController script.
in dit script sleep je elk puzzelstuk naar de lijst Draggable Objects en elk puzzel plek naar Snap Points.
De juiste combinaties van een puzzelplek en puzzelstuk worden bepaald door hun element in de lijst. 
Het puzzelstuk wat als Element 2 in de lijst staat bij Draggable Objects zal op de plek van Element 2 bij de SnapPoints vallen.

Hier zijn nog wat handige links die ik heb gebruikt voor het maken van dit onderdeel.
https://www.youtube.com/watch?v=axW46wCJxZ0

##################################################################################

Puzzelstukjes ontleden uit schematische tekeningen van de appendages:

Om dat te doen hebben wij het programma Gimp gebruikt (staat nog op de PC).
Op yt kan je verschillende tutorials vinden hoe je het programma het best kan gebruiken.

De schematische tekeningen staan in het mapje TataSteel/appendages.
In het mapje TataSteel/puzzelstukjes staan verschillende kleppen en kranen die wij alvast hebben ontleed. Het is waarschijnlijk niet alles maar
de meeste staat er al in.

Vervolgens kan je de stukjes in het project inporteren onder Assets/sprites/[naam van de kraan]. Zo hou je het ook overzichtelijk.

Infopaginas: 

De infopagina's zijn een soort van verwijzing naar het praktijkblok. Het is een simpele pagina waar je op het knop "verder kan drukken en wordt doorverwijzigd naar de quiz.
De layout is simpel en kan zo gekopieerd en geplakt worden om een nieuwe te maken, het enige wat je dan moet veranderen is de text en de link in de knop.
