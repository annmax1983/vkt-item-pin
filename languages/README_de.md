# VKT Item Pin

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine Browser-Erweiterung für die Produktrecherche: Erfasst Produkt-Snapshots per Mauszeiger. Titel, Preis, Link, Modell, Website und Datum werden in einer lokalen Bibliothek gespeichert – inklusive automatischer Preisverlaufs-Verfolgung.

> Chromium-basiert · Manifest V3 · Minimale Berechtigungen · Kein Tracking · 100 % lokal

---

## Warum VKT Item Pin?

Produktvergleiche über Einkaufsseiten hinweg bedeuten meist Dutzende offene Tabs und Copy-Paste in Tabellen. VKT Item Pin lässt Sie über ein Produkt fahren, **Pin** klicken und eine preisverfolgte Bibliothek direkt im Browser aufbauen.

| Vorteil | Detail |
|---------|--------|
| 🎯 **Erfassen per Hover** | Über ein Produkt fahren, Pin klicken – Titel, Preis, Link, Modell, Website und Datum werden automatisch extrahiert |
| 🔁 **Preis wird automatisch mitgeschrieben** | Eine bereits angepinnte Produktseite einfach erneut öffnen – der Preis wird ohne weiteren Klick erfasst |
| 🔔 **Lokaler Preisalarm** | Zielpreis pro Artikel festlegen: Beim ersten Erreichen oder Unterschreiten erscheint eine Desktop-Benachrichtigung – ohne Server, ohne E-Mail |
| 📈 **Preisverlauf** | Jede Erfassung – manuell oder automatisch – fügt einen Preispunkt hinzu und baut den Trend-Chart auf |
| 🛒 **24 Website-Voreinstellungen** | Feinabgestimmte Selektoren für Amazon, eBay, Etsy, Walmart, AliExpress, Temu u. v. m. – plus Universal-Engine (JSON-LD / OG / generische Selektoren) für alle anderen Shops |
| 🏷 **Notizen & Tags** | Begründung notieren („bis Black Friday warten“) und mit bis zu 10 Tags ordnen – beides durchsuchbar |
| 🖼️ **Vorschaubilder** | Produktbilder werden mit jedem Eintrag gespeichert |
| 🔒 **Privatsphäre zuerst** | Alle Daten bleiben über `chrome.storage.local` im Browser. Nichts wird hochgeladen |

---

## Funktionen

### 🆓 Kostenlos

| Funktion | Beschreibung |
|----------|--------------|
| 🎯 **Erfassen mit einem Klick** | Produkte auf Detailseiten oder in Suchergebnissen anpinnen |
| 📋 **Vorschau & Auswahl** | Felder vor dem Speichern bearbeiten; der „Auswahl“-Modus füllt Felder per Klick auf ein Seitenelement |
| 🔁 **Automatischer Preisverlauf** | Beim erneuten Öffnen einer angepinnten Produktseite wird der Preis im Hintergrund erfasst – ein Preispunkt pro Tag |
| 🔔 **Zielpreis-Alarm** | Zielpreis pro Artikel setzen; die Erfassung, die den Preis erstmals auf oder unter den Zielpreis bringt, löst eine Desktop-Benachrichtigung aus (rein lokal) |
| 📈 **Preisverlauf** | Unbegrenzte erneute Erfassungen bei verfolgten Produkten, mit Trend-Chart pro Artikel |
| 🏷 **Notizen & Tags** | Eine Notiz und bis zu 10 Tags pro Artikel – beides durchsuchbar und filterbar |
| 📊 **Bibliotheks-Statistik** | Zusammenfassung oben: Preissenkungen der letzten 30 Tage und Gesamtwert einer Bibliothek mit einer Währung |
| 🧭 **Anderswo vergleichen** | Mit einem Klick denselben Titel bei Google Shopping, eBay oder Amazon suchen |
| ✏️ **Einträge bearbeiten** | Titel/Modelle korrigieren, fehlerhafte Preispunkte ändern oder entfernen, Notizen, Tags und Zielpreis anpassen |
| 💾 **JSON-Backup** | Vollständige Bibliothek exportieren / importieren (offline nutzbar) – inklusive Notizen, Tags und Zielpreisen |
| 🧮 **Speicher-Monitor** | Zeigt die echte Speichernutzung und warnt frühzeitig |
| 🌍 **6 Sprachen** | Englisch, Chinesisch, Japanisch, Spanisch, Deutsch, Französisch |

### ⭐ Pro (Lizenz erforderlich)

| Funktion | Beschreibung |
|----------|--------------|
| ♾️ **Unbegrenzte Produkte** | Der Gratisplan umfasst 50 Produkte; Pro entfernt das Limit (erneute Erfassungen zählen nie mit) |
| 🔍 **Erweiterte Filter** | Nach Website, Tag, Zeitraum und Preisspanne filtern |
| 📤 **CSV-Export** | Langformat (eine Zeile pro Preispunkt, mit BOM, Excel-freundlich) inklusive Notizen, Tags und Zielpreis |
| 📊 **Produkte vergleichen** | Preisverläufe von bis zu 6 Produkten in einem Chart überlagern |

---

## Unterstützte Websites

**Manuell gepflegte Voreinstellungen (24):** Amazon (alle Marktplätze), eBay, Etsy, Walmart, Target, AliExpress, Temu, Best Buy, Home Depot, Lowe's, Newegg, Wayfair, Mercari, Shopee, Lazada, Rakuten, SHEIN, Alibaba.com / 1688, DHgate, TikTok Shop, bol.com, Allegro, Otto.de, Cdiscount …

**Alles andere** (Shopify / WooCommerce / unabhängige Shops) abdeckt die Universal-Engine: JSON-LD-strukturierte Daten → Open-Graph-Tags → generische Selektoren → Regex-Fallback → manueller Auswahlmodus.

---

## Installation

1. Erweiterungsseite öffnen: **Chrome** `chrome://extensions/` · **Edge** `edge://extensions/`
2. **Entwicklermodus** aktivieren (Schalter oben rechts)
3. Auf **Entpackte Erweiterung laden** klicken und den Ordner `vkt-item-pin` auswählen
4. Über ein beliebiges Produkt fahren und auf die 📌-Schaltfläche klicken

---

## Verwendung

### Produkt erfassen

1. Über ein Produkt fahren (Detailseite **oder** Suchergebnis-Raster) – die 📌-Schaltfläche erscheint
2. Klicken – ein Seitenpanel öffnet sich mit extrahiertem Titel, Preis, Link, Modell, Website und Datum
3. Anything korrigieren, mit **Auswahl** fehlende Felder ergänzen, dann **Speichern** klicken

### Preise verfolgen

- Ein bereits gespeichertes Produkt einfach erneut öffnen – der Preis wird automatisch erfasst, höchstens ein Punkt pro Tag (verfolgte Produkte zählen nie gegen das Gratislimit)
- Im Dashboard einen **Zielpreis** setzen: Bringt ein Besuch den Preis auf oder unter diesen Wert, erscheint eine Desktop-Benachrichtigung – einmal pro Überschreitung, ohne Wiederholungen
- Dashboard öffnen für Trend-Chart und 30-Tage-Bilanz oder **Vergleichen** (Pro) nutzen, um mehrere Produkte zu überlagern
- **Notiz** und **Tags** festhalten, warum sich Warten lohnt

### Backup

- Im Dashboard-Fuß: **JSON-Backup** / **Importieren** – regelmäßig empfohlen, da die Daten nur im Browser leben

---

## Privatsphäre

- `storage` — Speichert Ihre Bibliothek lokal. Kein Seiteninhalt verlässt den Browser.
- `scripting` + `activeTab` — Injizieren die Pin-Schaltfläche / extrahieren Felder nur bei Interaktion.
- `notifications` — Wird ausschließlich für lokale Zielpreis-Alarme genutzt. Es wird nichts gesendet.
- `<all_urls>` — Ermöglicht den Einsatz auf jeder Einkaufsseite. Liest oder lädt nie im Hintergrund Inhalte hoch.
- Kein Tracking, keine Analyse. Die einzige Netzwerkanfrage ist die Lizenzaktivierung/-prüfung bei Pro-Schlüsseln.

---

## Lizenz

Copyright © 2026 VKT Item Pin. Alle Rechte vorbehalten.

---

## ❤️ Unterstützen

Wenn Ihnen VKT Item Pin hilft, unterstützen Sie das Projekt!

**[👉 Lizenzschlüssel holen](https://www.annmax1983.com/checkout.html?plugin=itempin)** · [GitHub](https://github.com/annmax1983/ItemPin) · [Offizielle Website](https://www.annmax1983.com/extensions/itempin)
