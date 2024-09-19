<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Les cartes à retourner**</span> aident les gens à interagir avec une page web. Elles te permettent également de fournir des informations supplémentaires dans un espace réduit ou de cacher des informations qui ne devraient pas être directement visibles. Quelques exemples courants de cartes à retourner animées sont les cartes de révision, les cartes de visite, les cartes de contact des réseaux sociaux et les cartes de produits. 
</p>

Une carte à retourner comporte quatre parties principales :

- La carte elle-même
  - Le contrôle de retournement
    - Le recto de la carte
    - Le verso de la carte

Ajoute ce code à `index.html` pour positionner ta carte sur la page web :

--- code ---
---
language: html
filename: index.html
line_numbers: false

---
<div class="card"> <!-- La carte -->
    <div class="card-content"> <!-- Pour contrôler le retournement -->
        <div class="card-face"> <!-- Le recto de la carte -->
        <!-- Ajoute ici le contenu de ta carte de visite, y compris les images, le texte, etc -->
        </div>
      
        <div class="card-face flipme"> <!-- Le verso de la carte -->
        <!-- Ajoute ici le contenu de ta carte de visite, y compris les images, le texte, etc -->
        </div>
    </div>
</div>

--- /code ---

La carte à retourner utilise quatre classes CSS :

- `card`: définit la taille de la carte
- `card-content` : contrôle le timing, la perspective et l'effet de retournement
- `card-face`: cache la face de la carte lorsqu'elle est tournée vers l'arrière
- `flipme`: retourne la deuxième face de la carte de 180 degrés sur l'axe des y, de manière à ce qu'elle soit retournée dans la direction opposée à la première face de la carte

La classe `card-content` pivote de 180 degrés sur l'axe y lorsqu'elle est survolée, ce qui signifie que les deux faces de la carte changent de position.

## Personnaliser les faces de la carte

Tu peux ajouter du texte (y compris des emojis), des images, des citations ou des listes aux faces de tes cartes.

Tu peux appliquer une ou plusieurs classes de style, par exemple :

- `rounded`
- `xcenter` , `ycenter`
- `gradient1` , `gradient2`
- `dashed-border`, `solid-border`
- `primary` , `secondary` , `tertiary`

Un exemple de la manière de procéder est présenté ci-dessous :

--- code ---
---
language: html
filename: index.html
line_numbers: false

---
 <div class="card">
        <div class="card-content">
          <div class="card-face gradient1 rounded shadow">
            <img src="LapisSarawak02.png" alt="Lapis Sarawak" />
          </div>
          <div class="card-face flipme gradient2 rounded ycenter shadow">
            <h2>Lapis Sarawak</h2>
            <p>Un gâteau cuit en couches pour créer des motifs colorés.</p>
          </div>
        </div>
    </div>

--- /code ---

<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/web-flip-cards-example" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>

--- print-only ---

![Une bande d'exemples de cartes à retourner.](images/flip-example.png)

--- /print-only ---
