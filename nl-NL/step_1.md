<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Flip cards**</span> helpen mensen bij interactie met een webpagina. Ze maken het ook mogelijk om extra informatie in een kleine ruimte weer te geven of te verbergen zodat deze niet direct zichtbaar is. Sommige veel voorkomende voorbeelden van geanimeerde flip cards zijn revisie-kaarten, visitekaartjes, contactkaarten voor sociale media en productkaarten. 
</p>

Een flipcard bestaat uit vier hoofdonderdelen:

- De kaart zelf
  - De flip-control
    - De voorkant van de kaart
    - De achterkant van de kaart

Voeg deze code toe aan `index.html` om je kaart op de webpagina te plaatsen:

## --- code ---

language: html
filename: index.html
line_numbers: false

---

```
<div class="card"> <!-- De kaart -->
    <div class="card-content"> <! - Om de draaien -->
        <div class="card-face"> <! - De voorkant van de kaart-->
        <! - Voeg hier jouw inhoud toe voor de voorkant, inclusief afbeeldingen, tekst enz -->
        </div>
      
        <div class="card-face flipme"> <! - De achterkant van de kaart -->
        <! - Voeg hier je inhoud toe voor de achterkant, inclusief afbeeldingen, tekst enz -->
        </div>
    </div>
</div>
```

\--- /code ---

De flip card gebruikt vier CSS-klassen:

- `card`: stelt de grootte van de kaart in
- `card-content`: regelt de flip-timing, het perspectief en het effect
- `card-face`: verbergt de eerste kant wanneer deze naar achteren wordt gedraaid
- `flipme`: draait de tweede kaartzijde 180 graden om de y-as, zodat deze in de tegenovergestelde richting van de voorste kaartzijde wordt gedraaid

De klasse `card-content` draait 180 graden om de y-as wanneer je erover zweeft met je muis, wat betekent dat de twee kaartvlakken van positie wisselen.

## Pas de voor- en achterkant van de kaart aan

Je kunt tekst (inclusief emojis), afbeeldingen, citaten of lijsten aan je kaart toevoegen.

Je kunt een of meer stijlen toepassen zoals:

- `rounded`
- `xcenter` , `ycenter`
- `gradient1`, `gradient2`
- `dashed-border`, `solid-border`
- `primary` , `secondary` , `tertiary`

Hieronder zie je een voorbeeld van hoe je dit kunt doen:

## --- code ---

language: html
filename: index.html
line_numbers: false

---

```
 <div class="card">
        <div class="card-content">
          <div class="card-face gradient1 rounded shadow">
            <img src="LapisSarawak02.png" alt="Lapis Sarawak" />
          </div>
          <div class="card-face flipme gradient2 rounded ycenter shadow">
            <h2>Lapis Sarawak</h2>
            <p>Een cake die in lagen wordt gebakken om kleurrijke patronen te maken.</p>
          </div>
        </div>
    </div>
```

\--- /code ---

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/web-flip-cards-example" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>

\--- print-only ---

![Een strook met voorbeeld-flipcards.](images/flip-example.png)

\--- /print-only ---
