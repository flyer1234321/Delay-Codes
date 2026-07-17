# IATA Delay Codes – offline-app för iPhone/iPad

Sökbar referens för IATA delay codes (11–99). Fungerar helt offline efter första besöket.

## Funktioner

Snabbsökning på kodnummer, alfakod (t.ex. RA), svenska eller engelska ord – med smart rankning så att exakta koder alltid hamnar överst. Sökningen struntar i å/ä/ö (skriv "vader" så hittas "väder"). Kategorifilter per tiotal (10–19 … 90–99) med färgkodning. Språkväxling SV/EN (kommer ihåg ditt val). Tryck på ett kort för att se det andra språket och kopiera koden.

## Publicera på GitHub Pages

1. Skapa ett nytt repo på github.com, t.ex. `delay-codes`.
2. Ladda upp alla filer i den här mappen till repots rot (Add file → Upload files).
3. Gå till **Settings → Pages**. Under *Build and deployment*: Source = **Deploy from a branch**, Branch = **main**, mapp **/ (root)**. Spara.
4. Efter en minut finns appen på `https://DITT-ANVÄNDARNAMN.github.io/delay-codes/`.

## Installera på iPhone/iPad

1. Öppna adressen i **Safari**.
2. Tryck på **Dela**-knappen → **Lägg till på hemskärmen**.
3. Appen får en egen ikon och öppnas i helskärm utan Safari-gränssnitt.
4. Efter första öppningen fungerar den helt utan internet (service worker cachar allt).

## Uppdatera koderna

All data ligger i `index.html` i konstanten `DATA` (en rad per kod). Redigera, committa – och höj versionsnumret i `sw.js` (`delay-codes-v1` → `v2`) så hämtar telefonerna den nya versionen.

## Filer

`index.html` (hela appen, inkl. data), `sw.js` (offline-cache), `manifest.webmanifest` (hemskärmsapp), `icon-180/192/512.png` (ikoner).

Obs: Listan innehåller koderna 11–99. Serien 00–09 (interna flygbolagskoder) fanns inte med i källfilen – lägg gärna till dem i `DATA` om ni använder dem.
