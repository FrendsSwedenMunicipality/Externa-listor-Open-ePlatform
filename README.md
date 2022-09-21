# Externa listor för e-tjänsteplattformen Open ePlatform
Här finns några enklare externa listor för e-tjänsteplattformen Open ePlatform. Mest för att testa det nya kommunbiblioteket men hoppas att andra kommuner kan ha nytta av dessa.

En extern lista innebär att e-tjänsteplattformen inhämtar alternativen till kryssrute- och rullgardinslistor från andra system. Genom t.ex frends. Vissa listor kan ha stöd för attribut filtering när man vill inhämta olika alternativ beroende på vem som använder e-tjänsten eller andra attribut.

- [Heroma](#Heroma)
  - [Befattningskoder](#Befattningskoder)
  - [Lista med anställda](#Medarbetare)

Heroma
=====

## Befattningskoder
Läser in befattningar och befattningskoder från Heromas databas. <B>Observera</B> att fältnamn mm kan behöva anpassas i processen beroende på hur eran installation av heroma ser ut.

Listan har en direkt koppling mot Heromas databas men inget stöd för attribut filtrering.

<B>Miljövariablar</B>

| Variabelnamn                | Beskrivning                                             | Exempelvärde                                                         |
|-----------------------------|---------------------------------------------------------|----------------------------------------------------------------------|
| HeromaSQLConnectionstring   | sträng med inloggningsuppgifter till heromas databas    | Server=heromadb.kommunx;Database=Database_name;User Id=myUsername Password=myPass;

## Medarbetare
Lista med medarbetare med obligatorisk attributfiltering baserat på chefens användarnamn (vanligen den inloggade användaren i e-tjänsten men detta kan anpassas). 

<B>Miljövariablar</B>

| Variabelnamn                | Beskrivning                                             | Exempelvärde                                                         |
|-----------------------------|---------------------------------------------------------|----------------------------------------------------------------------|
| HeromaSQLConnectionstring   | sträng med inloggningsuppgifter till heromas databas    | Server=heromadb.kommunx;Database=Database_name;User Id=myUsername Password=myPass;

Parametrar:

| Variabelnamn      | Beskrivning            | Exempelvärde        |
|-------------------|------------------------|---------------------|
| username          | chefen användarnamn    | myUsername          |
