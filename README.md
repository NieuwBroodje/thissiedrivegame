# Thissie Drive: installeren via AltStore Classic

Dit project bouwt jouw game als iPhone-app (.ipa). Een .ipa maken kan alleen op een Mac of een Mac-server.
Daarom doet GitHub dat gratis voor je. Je hebt geen Mac nodig.

## Wat je nodig hebt
- Een gratis GitHub-account
- AltStore Classic op je telefoon, met AltServer draaiend op je pc of Mac (altstore.io)
- Een Apple ID (een gratis account is genoeg)

## Stap 1: de IPA laten bouwen
1. Maak op github.com een nieuwe, lege repository (privé mag).
2. Upload alle bestanden uit deze map, inclusief de verborgen map `.github`.
   Handig: pak de zip uit en sleep alles naar de pagina "uploading an existing file".
3. Ga in de repository naar **Actions**, kies **Bouw IPA voor AltStore** en klik op **Run workflow**.
4. Wacht ongeveer 5 tot 10 minuten tot het vinkje groen is.
5. Klik op de afgeronde run, scroll naar **Artifacts** en download **ThissieDrive-ipa**.
   Pak die zip uit: daarin zit `ThissieDrive.ipa`.

## Stap 2: op je telefoon zetten
1. Zet het .ipa-bestand op je telefoon (AirDrop, iCloud Drive of Bestanden).
2. Open AltStore, ga naar **My Apps** en tik op het **+** linksboven.
3. Kies `ThissieDrive.ipa`. AltStore tekent de app met jouw Apple ID en installeert hem.
4. Wil je de app laten verschijnen: Instellingen, Algemeen, VPN en apparaatbeheer, vertrouw jouw Apple ID.

## Goed om te weten
- Met een gratis Apple ID verloopt de app na 7 dagen. Open AltStore dan om te vernieuwen (AltServer moet op hetzelfde wifi draaien).
- Je mag maximaal 3 apps tegelijk geïnstalleerd hebben met een gratis Apple ID.
- Banen en tijden worden bewaard op de telefoon. Als je de app verwijdert, zijn ze weg.
- Multiplayer werkt in deze versie niet. Daarvoor is een eigen server nodig.
- De lettertypen worden van internet geladen. Zonder internet gebruikt de app een standaard lettertype.

## Zelf bouwen op een Mac (alternatief)
```
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```
Daarna in Xcode op Product, Archive klikken.
