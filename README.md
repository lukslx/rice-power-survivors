# Rice Power Survivors — L'assalto al Riso Supremo

**▶ Gioca subito: https://lukslx.github.io/rice-power-survivors/**

Un survivor-like / bullet-heaven in pixel art nello stile di *Vampire Survivors*, ambientato nell'universo di [Rice Power](https://lukslx.github.io/). Giri, il piccolo nigiri al salmone ribelle, deve resistere a orde infinite di creature affamate attirate dall'aroma irresistibile diffuso nel mondo dallo Chef Karaguashi.

> *"Non puoi scappare da tutti, Giri. Ma puoi resistere abbastanza a lungo da farli pentire di avere fame."* — Onigiri

Funziona nel browser su PC, tablet e telefono. Un solo file HTML, nessuna libreria, nessuna immagine o audio esterno: tutta la grafica è disegnata su Canvas e tutta la musica è sintetizzata con la Web Audio API.

## Come si gioca

Tu controlli **solo il movimento**: le armi attaccano da sole. Sopravvivi 15 minuti, raccogli i chicchi di riso lasciati dai nemici per salire di livello, scegli una carta a ogni livello e costruisci una combinazione di armi sempre più assurda. Allo scadere del tempo arriva il boss dello stage: sconfiggilo e raccogli il Chicco del Riso Supremo per sbloccare il mondo successivo.

- I **mini-boss** lasciano la **Ciotola Suprema**: potenziamenti gratuiti e **evoluzioni** (arma al livello 8 + passivo giusto = arma evoluta).
- Pickup: **Tonno XL** (cura), **Calamita di Nori** (attira tutti i chicchi), **Bomba di Soia** (spazza lo schermo), **Monete di Riso**.
- Tra una partita e l'altra spendi le monete nella **Dispensa di Onigiri** per potenziamenti permanenti.
- La **schivata** (dash) ha brevi frame di invulnerabilità e si può disattivare nelle opzioni.

### Controlli

| | PC | Touch |
|---|---|---|
| Movimento | WASD o frecce | joystick flottante (tocca e trascina dove vuoi) |
| Schivata | Shift o Spazio | pulsante SCHIVA |
| Pausa | Esc o P | pulsante ⏸ in alto a destra |
| Carte level-up | 1-2-3, frecce + Invio, o click | tocca la carta |
| Rilancia / Bandisci | R / B | pulsanti sotto le carte |

## Contenuti

**5 mondi**, gli stessi di Rice Power, ognuno con nemici, pericoli e boss propri:

1. **Città** — cittadini affamati, camerieri, gatti randagi, piccioni. Boss: *Il Maître Furioso*.
2. **Risaia di Montagna** — cervi che caricano, branchi di lupi, orsi. Boss: *Il Grande Orso della Risaia*.
3. **Isola del Vulcano** — pozze di lava e geyser; calamari di fuoco, serpenti velenosi, polli mitraglieri. Boss: *Tako Inferno*.
4. **Città Invasa** — barriere laser; alieni scout, laser e pesanti, droni, il Sushi Hunter. Boss: *Imperatore Gnam-Zor*.
5. **Karaguashi** — il pavimento ghiacciato del frigorifero, aiuto-cuochi, coltelli animati, piatti volanti e i sushi prigionieri da liberare, che diventano alleati. Boss finale: *Chef Karaguashi* in 3 fasi.

**5 personaggi**: Giri, Onigiri, Maki, Tempura e Supreme Giri (si sbloccano avanzando negli stage; l'ultimo battendo lo Chef).

**10 armi** con 8 livelli ciascuna (Pistola di Soia, Frusta di Alga Nori, Bacchette Rotanti, Zenzero Boomerang, Bomba Wasabi, Aura di Miso Bollente, Pioggia di Sesamo, Edamame Rimbalzante, Tempura Esplosiva, Razzo Rimbalzo), **6 evoluzioni** e **10 passivi**. Il ricettario delle evoluzioni è nel menu.

## Installazione come app

Il gioco è una PWA: aprendo il link su telefono o tablet si può aggiungere alla schermata Home ("Aggiungi a schermata Home") e giocare a tutto schermo, anche offline.

## Note tecniche

- Un unico `index.html` (HTML, CSS e JavaScript vanilla), più `manifest.json`, `sw.js` e le icone per la PWA.
- Risoluzione virtuale 384×216 scalata con pixel nitidi; font bitmap disegnato via codice.
- Object pooling e griglia spaziale per gestire centinaia di nemici e proiettili; qualità delle particelle adattiva se gli FPS calano.
- I progressi (monete, sblocchi, statistiche, opzioni) sono salvati nel browser in `localStorage` con prefisso `rps_`, separati da quelli di Rice Power. "Azzera progressi" è nelle opzioni.

Per giocare in locale basta aprire `index.html` nel browser. Per pubblicarlo basta copiare i file in un hosting statico (qui GitHub Pages).

## Crediti

Universo, personaggi e stile grafico derivano da **Rice Power**. Gioco progettato da Luca (lukslx) e sviluppato con l'aiuto di Claude (Anthropic).

---

*English:* a browser survivor-like / bullet-heaven set in the Rice Power universe, fully in Italian. Single self-contained HTML file, no dependencies, Canvas graphics and Web Audio synthesized music. Play it at https://lukslx.github.io/rice-power-survivors/
