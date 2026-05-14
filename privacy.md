---
title: Datenschutzerklärung
permalink: /privacy
---

# Datenschutzerklärung

**Status:** Draft
**Stand:** 2026-05-14
**Owner:** Christian Schreiber
**Verwendung:** Diese Datei ist die Markdown-Quelle. Vor Release wird sie als HTML auf GitHub Pages (oder vergleichbar) gehostet. Die App verlinkt aus dem Einstellungs-Screen auf die gehostete URL.

**TODO vor Release:** Adresse, Kontaktmail und Hosting-URL final einsetzen. Siehe `[PLATZHALTER:*]`-Markierungen.

---

## 1. Verantwortlicher

Verantwortlich für die Datenverarbeitung in dieser App im Sinne der Datenschutz-Grundverordnung (DSGVO) ist:

`[PLATZHALTER: Vollständiger Name oder Firma]`
`[PLATZHALTER: Adresse]`
`[PLATZHALTER: E-Mail-Adresse]`

Weitere Angaben findest du im [Impressum](impressum.md).

## 2. Zweck dieser App

Federchronik ist eine lokale Tagebuch-App für Füllfederhalter-Enthusiasten. Sie hilft, eigene Füller, Tinten, Papiere und Schreibeerfahrungen zu dokumentieren. Optional kann die App eine KI-Recherchefunktion nutzen, um technische Spezifikationen automatisch auszufüllen.

## 3. Welche Daten werden verarbeitet?

### 3.1 Lokal auf deinem Gerät

Folgende Daten speichert Federchronik ausschließlich lokal auf deinem iPhone:

- Deine eingegebenen Füller-, Tinten- und Papierdaten (Hersteller, Modell, Notizen, Bilder)
- Deine Tagebuch-Einträge (Bewertungen, Notizen, Fotos)
- Dein Anthropic-API-Key (verschlüsselt in der iOS-Keychain)
- App-Einstellungen

Diese Daten verlassen dein Gerät nicht, außer in dem ausdrücklich beschriebenen Fall in Abschnitt 3.2.

### 3.2 Übermittlung an Anthropic (nur bei aktiver Nutzung der KI-Recherche)

Wenn du in der App den „Recherchieren"-Button für einen Füller oder eine Tinte verwendest, sendet die App folgende Daten an die Anthropic-API (`api.anthropic.com`):

- Den von dir eingegebenen Hersteller- und Produktnamen
- Deinen Anthropic-API-Key zur Authentifizierung
- Ein deutschsprachiges Prompt-Template, das Anthropic bittet, Spezifikationen zu recherchieren

**Wichtig:** Anthropic ist ein Anbieter mit Sitz in den USA. Bei jeder KI-Recherche findet eine Drittland-Datenübermittlung in die USA statt.

Die Vertragsbeziehung zur Datenverarbeitung durch Anthropic besteht zwischen *dir* (als Anthropic-Account-Inhaber) und Anthropic. Federchronik ist nicht Auftragsverarbeiter im Sinne von Art. 28 DSGVO. Die Rechtsgrundlage dieser Übermittlung ist deine Einwilligung durch Nutzung der KI-Recherchefunktion (Art. 6 Abs. 1 lit. a DSGVO).

Bitte beachte die Datenschutzerklärung von Anthropic: <https://www.anthropic.com/legal/privacy>.

### 3.3 Was wir *nicht* verarbeiten

- Wir haben kein Backend und betreiben keine eigenen Server für die App
- Wir nutzen keine Analytics-, Tracking- oder Werbe-SDKs
- Wir sammeln keine Telemetrie-Daten
- Wir haben keinen Zugriff auf deinen Anthropic-API-Key, deine Sammlungsdaten oder deine Fotos
- Wir setzen keine Cookies (es gibt keinen Web-Anteil)

## 4. Rechte als betroffene Person

Da Federchronik selbst keine personenbezogenen Daten zentral verarbeitet, bestehen folgende Rechte direkt gegenüber dem Verantwortlichen für die Datenverarbeitung — das bist im Wesentlichen du selbst (lokale Daten) und Anthropic (bei aktivem KI-Research):

- **Auskunftsrecht (Art. 15 DSGVO):** Deine lokalen Daten kannst du direkt in der App einsehen. Für bei Anthropic gespeicherte Daten wende dich an Anthropic über deinen Account.
- **Recht auf Berichtigung (Art. 16 DSGVO):** Bearbeite deine Einträge direkt in der App.
- **Recht auf Löschung (Art. 17 DSGVO):** Lösche Einträge in der App oder deinstalliere die App komplett, um alle lokalen Daten zu entfernen.
- **Recht auf Datenübertragbarkeit (Art. 20 DSGVO):** Eine Exportfunktion ist in 1.0 nicht implementiert (siehe Roadmap).
- **Beschwerderecht (Art. 77 DSGVO):** Du kannst dich bei einer Datenschutz-Aufsichtsbehörde beschweren, in Deutschland z. B. beim Bundesbeauftragten für den Datenschutz und die Informationsfreiheit (BfDI).

## 5. App-Berechtigungen

Federchronik fragt während der Nutzung folgende iOS-Berechtigungen an:

- **Fotomediathek (PhotoKit):** ausschließlich zum Auswählen von Bildern für Tagebuch-Einträge. Die App nutzt nur ausgewählte Bilder (keine Zugriff auf die gesamte Mediathek).
- **Netzwerk:** ausschließlich, um die Anthropic-API zu erreichen, wenn du KI-Recherche nutzt.

Die App fragt **keine** Berechtigungen für Standort, Kontakte, Kalender, Mikrofon, Tracking oder Benachrichtigungen an.

## 6. Speicherdauer

Lokale Daten bleiben gespeichert, bis du sie in der App löschst oder die App deinstallierst.

Daten, die im Rahmen der KI-Recherche an Anthropic übermittelt wurden, unterliegen der Aufbewahrungsfrist von Anthropic gemäß deren Datenschutzerklärung.

## 7. Sicherheit

- Dein Anthropic-API-Key wird in der iOS-Keychain gespeichert mit der Schutzklasse `kSecAttrAccessibleAfterFirstUnlockThisDeviceOnly`. Das bedeutet: der Key ist nur nach dem ersten Entsperren deines iPhones nach einem Neustart verfügbar und wird **nicht** in iCloud-Backups oder in den iCloud-Keychain übertragen.
- Deine Sammlungsdaten liegen in einem SwiftData-Store mit iOS Data Protection (`NSFileProtectionComplete`).
- Die Kommunikation mit der Anthropic-API findet ausschließlich über HTTPS mit aktueller TLS-Verschlüsselung statt.

## 8. Änderungen dieser Datenschutzerklärung

Diese Erklärung wird angepasst, wenn sich die Funktionsweise der App ändert. Die aktuelle Fassung ist immer unter `https://federchronik.scribendo.de/privacy` (Subdomain wird im Rahmen von Roadmap Phase 6 eingerichtet) abrufbar.

---

**Stand:** 2026-05-14
