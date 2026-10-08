# Wortblitz

Ein deutsches Wortratespiel im Stil von Wordle, als einzelne HTML-Datei ohne Abhängigkeiten.

Errate das Wort mit 5 Buchstaben in 6 Versuchen. Nach jedem Versuch zeigt die Farbe, wie nah du dran bist:

- 🟩 richtiger Buchstabe an der richtigen Stelle
- 🟨 Buchstabe kommt vor, steht aber woanders
- ⬛ Buchstabe kommt nicht vor

## Spielen

`index.html` im Browser öffnen, fertig. Es wird weder ein Build noch ein Server noch eine Internetverbindung gebraucht.

## Funktionen

- **Tageswort**, das für alle am selben Datum gleich ist, und beliebig viele **Zufallswörter**
- **Wörterbuchprüfung**: Eingaben, die kein deutsches Wort sind, werden abgelehnt und kosten keinen Versuch
- **Statistik** mit Siegquote, Serie und Verteilung der Versuche
- **Ergebnis teilen** als Emoji-Raster ohne Spoiler, per Zwischenablage oder Teilen-Menü am Handy
- **Gespeicherter Tagesstand**: Neuladen oder Schließen verliert weder den Fortschritt noch das Ergebnis
- Eingabe per Tastatur oder Bildschirmtastatur, Umlaute (Ä, Ö, Ü) inklusive; ß wird als SS geschrieben

Statistik und Spielstand liegen im `localStorage` des Browsers. Es werden keine Daten übertragen.

## Wortlisten

- Es gibt rund 540 Lösungswörter. Sie stehen in `index.html` in der Konstante `WORDS`.
- Als gültige Eingaben dienen rund 4.500 Wörter in der Konstante `VALID`. Sie stammen aus dem deutschen Systemwörterbuch `ngerman` und enthalten alle Lösungswörter.
- Das Wörterbuch ist nicht vollständig. Moderne Begriffe oder Fremdwörter werden unter Umständen zu Unrecht abgelehnt.

## Lizenz

[MIT](LICENSE)
