# TA Swiss Starter Map

Basiert auf dem Starterkit von WorkAdventure / [WorkAdventure](https://workadventu.re).

Um zu verstehen, wie man dieses Starterkit benutzt, folgt der Anleitung unter [https://workadventu.re/map-building](https://workadventu.re/map-building).

## Structure
* *public*: Static files like PDFs or audio files
* *src*: Scripts files
* *tilesets*: All tilesets
* *map.tmj*: Map file
* *map.png*: The map thumbnail displayed on the in-game map information / we recommend using 500x500 images for the map thumbnails.

Wenn du mehr als eine Map-Datei verwenden möchtest, füge die neue Map-Datei einfach im Stammverzeichnis oder in einem Ordner hinzu.

Wenn du benutzerdefinierte Webseiten erstellst, um sie in die Karte einzubetten, verweise bitte auf die HTML-Dateien im Ordner `input` option in *vite.config.js*.

## Requirements

Node.js version >=17

## Clone to Desktop

1. GitHub Desktop installieren (https://desktop.github.com/)
2. Zum jeweiligen Repository in den Tab 'Code' switchen
3. Dort auf das Dropdown Menu bei 'Code' auf 'Open with Github Pages'

![image](https://github.com/dezentrum/ta_swiss/assets/69964846/d9b4b1e0-849e-4b82-a607-8fcfebb06fb2)

4. Wenn gefragt, das Repository 'Clonen' - das sorgt dafür, dass es eine lokale Kopie auf deinem Laptop vom Code aus Github gibt.
   
![image](https://github.com/dezentrum/ta_swiss/assets/69964846/ddd036c2-8c00-40cb-ac73-2034e18286ae)

6. Dem Tutorial von WorkAdventure weiter folgen (https://docs.workadventu.re/map-building/tiled-editor/#loading-the-map-in-tiled)

## Installation

With npm installed (comes with [node](https://nodejs.org/en/)), run the following commands into a terminal in the root directory of this project:

```shell
npm install
npm run dev
```

## Test production map

You can test the optimized map as it will be in production:
```sh
npm run build
npm run prod
```

## Licenses

This project contains multiple licenses as follows:

* [Code license](./LICENSE.code) *(all files except those for other licenses)*
* [Map license](./LICENSE.map) *(`map.tmj` and the map visual as well)*
* [Assets license](./LICENSE.assets) *(the files inside the `src/assets/` folder)*

### About third party assets

If you add third party assets in your map, do not forget to:
1. Credit the author and license with the "tilesetCopyright" property present in the properties of each tilesets in the `map.tmj` file
2. Add the license text in LICENSE.assets
