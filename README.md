# MTG PriceCam

Web app d’una sola pàgina que escaneja amb la càmera el **codi de la part inferior esquerra** de cartes de Magic (p. ex. `039/302 C`), fa **OCR** amb Tesseract.js i consulta **Scryfall** per mostrar el **preu** (EUR/USD) automàticament.

- 🔎 OCR automàtic de la zona inferior esquerra (i gir 180°)
- 🎥 Funciona amb la càmera del navegador (HTTPS/localhost)
- 💶 Llindar d’alerta amb so si supera un valor
- 🧪 Sense frameworks: HTML + JS pur + Tesseract.js

## Prova-ho
https://unamedarwin.github.io/mtg-pricecam/

## Ús
1. Obre la pàgina i prem **Inicia càmera**.  
2. Passa cartes davant del visor; si detecta un codi tipus `NNN/NNN X`, consulta Scryfall i mostra el **preu**.  
3. Opcional: marca “preferir cartes en espanyol” i ajusta el **llindar d’alerta (€)**.

## Fitxers
- `index.html` – tota l’app (HTML + CSS + JS).  
  Inclou Tesseract per CDN i crides a l’API pública de Scryfall.

## Tecnologies
- [Tesseract.js](https://github.com/naptha/tesseract.js) (OCR)
- [Scryfall API](https://scryfall.com/docs/api) (dades i preus)

## Llicència
MIT
