---
title: Impressum
permalink: /impressum
---

# Impressum

**Status:** Draft
**Stand:** 2026-05-14
**Owner:** Christian
**Verwendung:** Diese Datei ist die Markdown-Quelle. Vor Release wird sie als HTML auf GitHub Pages (oder vergleichbar) gehostet. Die App verlinkt aus dem Einstellungs-Screen auf die gehostete URL.

**TODO vor Release:** Adresse final einsetzen, Entscheidung Privatadresse / Impressum-Service / c/o AutoCompliance treffen. Siehe `[PLATZHALTER:*]`-Markierungen und ADR-0005 (Individual vs. Organization).

---

## Angaben gemäß § 5 TMG / § 18 MStV

`[PLATZHALTER: Vollständiger Name oder Firma]`
`[PLATZHALTER: Straße + Hausnummer]`
`[PLATZHALTER: PLZ + Ort]`
Deutschland

## Kontakt

E-Mail: `[PLATZHALTER: E-Mail-Adresse]`

## Verantwortlich für den Inhalt nach § 18 Abs. 2 MStV

`[PLATZHALTER: Vollständiger Name]`
`[PLATZHALTER: Adresse — kann mit der oben genannten identisch sein]`

## Umsatzsteuer-Identifikationsnummer

`[PLATZHALTER bei Firma: USt-ID gem. § 27a UStG]`

Bei rein privater, nicht-gewerblicher Veröffentlichung der App entfällt dieser Abschnitt.

## Haftungsausschluss

### Haftung für Inhalte

Die Inhalte der App werden mit größtmöglicher Sorgfalt erstellt. Für die Richtigkeit, Vollständigkeit und Aktualität der von der App über die Anthropic-API ausgegebenen KI-Recherche-Ergebnisse kann keine Gewähr übernommen werden. Diese Ergebnisse sind Hilfestellung, kein Garantie-Datenblatt.

### Haftung für Links

Die App enthält ggf. Links zu externen Websites Dritter (z. B. Anthropic-Konsole). Auf deren Inhalte hat der Anbieter keinen Einfluss; eine Haftung für diese fremden Inhalte wird nicht übernommen.

### Urheberrecht

Die durch den Anbieter erstellten Inhalte und Werke (App-Code, Texte) unterliegen dem deutschen Urheberrecht. Beiträge Dritter sind als solche gekennzeichnet (siehe [Third-Party Licenses](third-party-licenses.md)).

---

**Stand:** 2026-05-14

## Diskussions-Notiz (intern, nicht für Hosting)

ADR-0005 hat geklärt: Federchronik läuft als Individual-Account auf Christian persönlich. Damit ist Christian als Privatperson Impressum-Verantwortlicher. AutoCompliance GmbH und Scribendo GmbH kommen nicht als Impressum-Träger in Frage, weil sie nicht Owner der App sind.

Zwei verbleibende Optionen für die Adress-Zeile:

1. **Privatadresse**: günstig (0 €), aber öffentlich sichtbar
2. **Impressum-Service** (z. B. impressum-service.de): ~5–10 €/Monat, Adresse des Anbieters mit Weiterleitung

Diese Entscheidung wird vor dem App-Store-Release endgültig getroffen und in einer Folge-ADR (`docs/decisions/0007-impressum-adresse.md`) dokumentiert.

## Hosting

Diese Datei wird als HTML unter `https://federchronik.scribendo.de/impressum` gehostet (Subdomain auf der Domain `scribendo.de`, die einer vermögensverwaltenden GmbH von Christian gehört — die GmbH ist *nicht* Impressum-Verantwortliche, sondern nur Domain-Inhaberin). DNS- und GitHub-Pages-Setup siehe Roadmap Phase 6.
