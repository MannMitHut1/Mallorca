# Apartment 422 · Santa Ponsa

Statische Info-Seite zum Apartment – für Freunde und Familie.
Kein Build, kein Framework, keine externen Abhängigkeiten (keine Google Fonts,
kein JavaScript). Nur HTML, eine CSS-Datei und Bilder.

## Seiten

| Datei | Inhalt |
| --- | --- |
| `index.html` | Startseite mit Kacheln und horizontaler Galerie (Vollbild beim Antippen) |
| `expose.html` | Apartment, CAESARS, Umgebung, Anfahrt, Kontakt |
| `infos.html` | Versorgung, WLAN, Baden, Mobilität, Baby, House Rules |
| `ausstattung.html` | Küche, Möbel, Wäsche, Technik, Unterhaltung, Strand-Equipment, Baby |
| `checkin.html` | Check-in-Liste |
| `checkout.html` | Check-out-Liste |
| `impressum.html` | Impressum |
| `datenschutz.html` | Datenschutzhinweise |

Bilder liegen in `bilder/`, das Styling komplett in `style.css`. Die Seite kommt
ohne eine Zeile JavaScript aus.

Jede Seite trägt eine Content Security Policy (`default-src 'none'`), die nur
Inhalte aus dem eigenen Verzeichnis zulässt – fremde Skripte, Schriften oder
Zählpixel können also nicht nachgeladen werden, auch nicht versehentlich.
Dazu `referrer: no-referrer`, damit die Adresse der Seite beim Klick auf einen
externen Link nicht weitergegeben wird.

## Veröffentlichen mit GitHub Pages

1. Im Repository auf **Settings → Pages** gehen.
2. Unter *Source* **Deploy from a branch** wählen.
3. Als Branch den gewünschten Branch und den Ordner `/ (root)` auswählen, dann **Save**.
4. Nach ein bis zwei Minuten ist die Seite unter
   `https://<benutzername>.github.io/Mallorca/` erreichbar.

`.nojekyll` schaltet die Jekyll-Verarbeitung ab, `robots.txt` und ein
`noindex`-Meta-Tag halten die Seite aus Suchmaschinen heraus.

## Hinweis

Eine über GitHub Pages veröffentlichte Seite ist öffentlich erreichbar, auch wenn
das Repository privat ist – jeder mit der Adresse kann sie sehen. Auf der Seite
stehen keine Zugangsdaten und keine privaten Telefonnummern: Das WLAN-Passwort
gibt Florian persönlich weiter, ebenso die Notfall-Nummern.
