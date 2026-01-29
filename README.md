# ETF-Vorsorgeplaner und Inflationsrechner

Dieses Repository enthält ein interaktives Python-Notebook zur finanziellen Aufklärung. Es dient dazu, die Auswirkungen der Inflation auf die zukünftigen Lebenshaltungskosten zu visualisieren und die Effektivität von langfristigen ETF-Investitionen mittels Zinseszinseffekt aufzuzeigen.

## Projektziel

Das primäre Ziel dieses Projekts ist die Visualisierung komplexer finanzmathematischer Zusammenhänge:
* **Bedarfsanalyse:** Aufzeigen des nominalen Kapitalbedarfs im Alter unter Berücksichtigung verschiedener Inflationsszenarien.
* **Rentenlücke:** Darstellung der Differenz zwischen dem zukünftigen Bedarf und der erwarteten gesetzlichen Rente.
* **Zinseszins-Hebel:** Verdeutlichung des Verhältnisses zwischen Eigenleistung (Einzahlungen) und Marktwachstum (Zinseszins).

## Nutzung der Entwicklungsumgebung

Das Projekt ist für die Nutzung mit Visual Studio Code und Docker optimiert, um eine konsistente Laufzeitumgebung zu gewährleisten.

### Voraussetzungen

* Docker Desktop
* Visual Studio Code
* VS Code Extension: Dev Containers

### Inbetriebnahme

1. Das Repository lokal klonen oder herunterladen.
2. Den Ordner in Visual Studio Code öffnen.
3. Beim Erscheinen der Benachrichtigung "Reopen in Container" bestätigen.
4. Falls die Benachrichtigung nicht erscheint: Befehlspalette öffnen (Strg+Umschalt+P), "Dev Containers: Reopen in Container" wählen.
5. Die Datei vorsorgeplaner.ipynb öffnen und alle Zellen ausführen.

## Struktur der Berechnungen

### 1. Kaufkraft-Prognose und Rentenlücke
In diesem Modul wird berechnet, wie sich heutige Lebenshaltungskosten über die Zeit entwickeln. Optional kann eine erwartete Rente definiert werden, um die resultierende monatliche Deckungslücke zum Rentenbeginn zu identifizieren.

### 2. ETF-Investitionsrechner
Dieses Modul nutzt die Daten aus der Bedarfsanalyse, um eine Investmentstrategie zu simulieren. Es berücksichtigt:
* Jährliche Dynamik der Sparrate zur Kompensation von Inflation und Gehaltssteigerungen.
* Steuerliche Aspekte der Entnahmephase (Abgeltungssteuer-Näherung inklusive Teilfreistellung).
* Darstellung des Kapitals bis zum Ende der statistischen Lebenserwartung.

## Mathematische Grundlagen

* **Nominaler Bedarf:** Berechnung mittels Zinseszinsformel $K_n = K_0 \cdot (1 + i)^n$.
* **Besteuerung:** Anwendung eines effektiven Steuersatzes von 18% auf den Gewinnanteil der Entnahmen (entspricht der deutschen Abgeltungssteuer für Aktienfonds nach 30% Teilfreistellung).
* **Zins-Inflection-Point:** Identifikation des Zeitpunkts, an dem die monatlichen Zinserträge die eigenen Einzahlungen übersteigen.

## Rechtlicher Hinweis

Die Berechnungen dienen ausschließlich der allgemeinen Aufklärung und stellen keine Anlageberatung oder Finanzplanung dar. Alle Ergebnisse sind Modellrechnungen basierend auf Benutzereingaben und hypothetischen Renditeannahmen.