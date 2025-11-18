# Wochenplaner - Anwesenheitsverwaltung

## 📋 Was ist der Wochenplaner?

Der Wochenplaner ist eine browserbasierte Anwendung zur Verwaltung von Schüler-Anwesenheiten während Ferienzeiten. Die Anwendung läuft komplett im Browser und speichert alle Daten in .json-Dateien auf deinem Computer.

---

## 🚀 Erste Schritte

### 1. Anwendung öffnen

Öffne die Datei `Klasse4.html` in einem modernen Browser:
- **Empfohlen:** Google Chrome, Microsoft Edge, Opera
- **Funktioniert mit Einschränkungen:** Firefox (kein File System Access, nur Drag & Drop)
- **Nicht unterstützt:** Ältere Browser (Internet Explorer)

### 2. Datei laden oder erstellen

Beim ersten Start hast du zwei Möglichkeiten:

#### Option A: Neue Planung erstellen
1. Klicke auf **"Planung öffnen / Neue erstellen"**
2. Wähle **"Neue leere Planung erstellen"**
3. Gib einen Dateinamen ein (z.B. `ferienplanung_2025.json`)
4. Wähle einen Speicherort auf deinem Computer
5. Die Datei wird erstellt und automatisch geöffnet

#### Option B: Bestehende Planung laden
1. Klicke auf **"Planung öffnen / Neue erstellen"**
2. Wähle **"Bestehende Planung laden"**
3. Wähle eine vorhandene .json-Datei aus
4. Die Daten werden geladen

#### Option C: Drag & Drop (schnellste Methode)
1. Ziehe eine .json-Datei direkt auf die Browser-Seite
2. Die Datei wird automatisch geladen
3. ⚠️ **Wichtig:** Bei Drag & Drop werden Änderungen NICHT automatisch gespeichert! Nutze "Backup erstellen" um zu speichern.

---

## 📊 Grundfunktionen

### Dateiname-Anzeige

Im Header siehst du unter "Wochenplaner" den aktuell geladenen Dateinamen:
- 📄 **Grün:** Datei ist geladen (z.B. `📄 ferienplanung_2025.json`)
- **Grau:** Keine Datei geladen

### Klassen verwalten

Die Anwendung unterstützt 4 Klassen:
1. Wähle im Dropdown-Menü die gewünschte Klasse aus
2. Jede Klasse hat ihre eigenen Personen und Anwesenheitsdaten
3. Die Daten aller Klassen werden in einer gemeinsamen .json-Datei gespeichert

### Wochen navigieren

- **◄ (Pfeil links):** Vorherige Woche anzeigen
- **► (Pfeil rechts):** Nächste Woche anzeigen
- **Schnellnavigation:** Springe direkt zu einem Sondertag über das Dropdown-Menü

---

## 👥 Personen verwalten

### Person hinzufügen

1. Scrolle zur letzten (leeren) Zeile der Tabelle
2. Gib den Namen in das Textfeld ein (z.B. "Max Mustermann")
3. Drücke **Enter** oder klicke außerhalb des Feldes
4. Die Person wird automatisch gespeichert

### Person umbenennen

1. Klicke auf den Namen in der Tabelle
2. Ändere den Namen
3. Klicke außerhalb des Feldes oder drücke **Enter**
4. Die Änderung wird automatisch gespeichert

### Person löschen

1. Klicke auf das **Papierkorb-Symbol** (🗑️) in der Zeile der Person
2. Bestätige die Sicherheitsabfrage
3. Die Person und alle zugehörigen Anwesenheitsdaten werden gelöscht

---

## ✅ Anwesenheit markieren

### Wichtig zu verstehen:
- **Checkboxen sind nur an Ferientagen aktiviert**
- An normalen Schultagen sind Checkboxen ausgegraut
- Eine **aktivierte Checkbox** bedeutet: "Person ist anwesend/nimmt teil"

### Anwesenheit markieren

1. Stelle sicher, dass Ferientage definiert sind (siehe unten)
2. Klicke auf die Checkbox neben dem Namen an einem Ferientag
3. Die Anwesenheit wird automatisch gespeichert

### Alle Ferientage einer Woche markieren

1. Klicke auf das **Häkchen-Symbol** (✓) in der Zeile einer Person
2. Alle Ferientage der aktuellen Woche werden für diese Person markiert

---

## 📅 Sondertage verwalten (Ferien/Feiertage)

### Sondertage-Dialog öffnen

Klicke auf **"Sondertage"** im Header

### Ferienzeit hinzufügen

1. Gib einen **Namen** ein (z.B. "Herbstferien 2025")
2. Wähle den **Typ:**
   - **Ferien:** Checkboxen sind aktiviert, Anwesenheit kann markiert werden
   - **Geschlossen:** Checkboxen sind deaktiviert (z.B. für Schließzeiten)
3. Wähle **Startdatum** und **Enddatum**
4. Optional: Füge einen **zusätzlichen Feiertag** hinzu (z.B. "Ostermontag")
5. Klicke auf **"Hinzufügen"**

### Beispiel: Osterferien mit Feiertag

- **Name:** Osterferien 2025
- **Typ:** Ferien
- **Startdatum:** 07.04.2025
- **Enddatum:** 18.04.2025
- **Zusätzlicher Feiertag:**
  - Name: Ostermontag
  - Datum: 21.04.2025

### Sondertag löschen

1. Öffne den Sondertage-Dialog
2. Klicke auf das **Papierkorb-Symbol** (🗑️) neben dem Eintrag
3. Der Sondertag wird gelöscht

---

## 💾 Speichern und Sichern

### Automatisches Speichern (Autosave)

- **Nur wenn Datei über "Planung öffnen" geladen wurde**
- Änderungen werden automatisch nach 1,5 Sekunden gespeichert
- Du siehst eine **"Gespeichert!"** Meldung oben in der Mitte

### Backup erstellen

1. Klicke auf **"Backup erstellen"** im Header
2. Wähle einen Speicherort
3. Die Datei wird mit Präfix `backup_wochenplaner_...` gespeichert
4. Bestätigung erscheint: "Backup erfolgreich erstellt!"

**Wann solltest du ein Backup erstellen?**
- Vor größeren Änderungen
- Regelmäßig (z.B. wöchentlich)
- Bevor du die Anwendung auf einem anderen Rechner öffnest
- Nach Drag & Drop (da kein Autosave)

---

## 📊 Export nach Excel

### Anwesenheitsliste exportieren

1. Klicke auf den grünen **"Export (Excel)"** Button unten rechts
2. Gib einen Dateinamen ein (z.B. `Anwesenheit_Januar_2025.xlsx`)
3. Klicke auf **OK**
4. Die Excel-Datei wird heruntergeladen

### Was enthält die Excel-Datei?

Die exportierte Excel-Datei enthält mehrere Tabellenblätter:

1. **Rohdaten:**
   - Alle Anwesenheiten mit Klasse, Vorname, Nachname, Datum

2. **Anzahl pro Woche:**
   - Übersicht: Wie viele Personen pro Wochentag anwesend waren
   - Summe pro Woche

3. **KW [Nummer]:**
   - Ein Blatt pro Kalenderwoche
   - Namen aufgeteilt nach Wochentagen
   - Ideal zum Ausdrucken

---

## 🎨 Dark Mode / Light Mode

Klicke auf das **Mond/Sonne-Symbol** (🌙/☀️) im Header um zwischen hellem und dunklem Design zu wechseln.

Die Einstellung wird im Browser gespeichert.

---

## ⚠️ Wichtige Hinweise

### Datenspeicherung

- **Alle Daten werden in .json-Dateien auf deinem Computer gespeichert**
- **Browser-Cache wird beim Schließen gelöscht** (keine Daten im Browser!)
- **Sichere deine .json-Datei regelmäßig** (z.B. auf USB-Stick, Cloud)

### Browser-Kompatibilität

| Browser | Autosave | Drag & Drop | Backup |
|---------|----------|-------------|--------|
| Chrome | ✅ | ✅ | ✅ |
| Edge | ✅ | ✅ | ✅ |
| Opera | ✅ | ✅ | ✅ |
| Firefox | ❌ | ✅ | ✅ |
| Safari | ⚠️ | ✅ | ⚠️ |

**Firefox:** File System Access API nicht unterstützt → Nutze Drag & Drop + Backup

### Fehlerbehebung

**Problem:** "Fehler beim Speichern!"
- **Lösung:** Erstelle sofort ein Backup über "Backup erstellen"
- **Ursache:** Möglicherweise wurde die Datei gelöscht oder verschoben

**Problem:** Checkboxen sind ausgegraut
- **Lösung:** Definiere Ferientage über "Sondertage"
- **Ursache:** Checkboxen sind nur an Ferientagen aktiviert

**Problem:** Drag & Drop funktioniert nicht
- **Lösung:** Stelle sicher, dass du eine .json-Datei verwendest
- **Alternative:** Nutze "Planung öffnen / Neue erstellen"

**Problem:** Daten sind nach Browser-Neustart weg
- **Lösung:** Du hast keine .json-Datei geladen
- **Wichtig:** Beim nächsten Mal "Planung öffnen" oder Drag & Drop nutzen

---

## 📝 Workflow-Beispiel

### Szenario: Herbstferien-Planung für Klasse 3

1. **Anwendung öffnen:** `Klasse4.html` im Browser öffnen
2. **Datei erstellen:** "Neue leere Planung erstellen" → `herbstferien_2025.json`
3. **Klasse wählen:** "Klasse 3" im Dropdown auswählen
4. **Ferien definieren:**
   - "Sondertage" öffnen
   - Name: "Herbstferien 2025"
   - Typ: "Ferien"
   - Datum: 06.10.2025 - 17.10.2025
   - "Hinzufügen"
5. **Personen hinzufügen:**
   - "Anna Schmidt"
   - "Max Müller"
   - "Lisa Weber"
6. **Zur ersten Ferienwoche navigieren:**
   - Schnellnavigation → "Herbstferien 2025"
7. **Anwesenheit markieren:**
   - Anna: Montag, Mittwoch, Freitag
   - Max: Alle Tage (Häkchen-Symbol nutzen)
   - Lisa: Dienstag, Donnerstag
8. **Backup erstellen:**
   - "Backup erstellen" → `backup_wochenplaner_2025-10-01.json`
9. **Excel exportieren:**
   - "Export (Excel)" → `Herbstferien_Anwesenheit.xlsx`

---

## 🆘 Support & Fragen

Bei Problemen oder Fragen:
1. Überprüfe diese Anleitung
2. Stelle sicher, dass du einen unterstützten Browser verwendest
3. Erstelle regelmäßig Backups deiner Daten

---

**Version:** 2.0
**Letzte Aktualisierung:** November 2025
**Kompatibilität:** Chrome 90+, Edge 90+, Opera 76+, Firefox 88+ (eingeschränkt)
