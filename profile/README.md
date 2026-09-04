<!-- GENERIERTE DATEI - NICHT IM REPO ".github" BEARBEITEN.
     Quelle: BieLeMetrics-Website/org-profile/README.md
     Die Synchronisation macht .github/workflows/sync-org-profile.yml. -->
<h1 align="center">BieLeMetrics</h1>

<p align="center">
  <b>Erwartete Tore und Paraden im Profihandball – live.</b><br>
  <a href="https://bielemetrics.de">bielemetrics.de</a>
</p>

---

BieLeMetrics berechnet **xGoals (xG)** und **xSaves (xS)** für Handballspiele:
für jeden Wurf die Wahrscheinlichkeit, dass er im Tor landet – und daraus, wie
gut Spieler ihre Chancen nutzen und wie gut Torhüter die zugelassenen Würfe
halten. Rohe Trefferquoten belohnen leichte Würfe; Erwartungswerte rechnen die
Schwierigkeit der Situation heraus und machen Leistungen vergleichbar.

Die Kennzahlen entstehen **während des Spiels**, aus synchronisierten
Positions- und Eventdaten, und gehen automatisiert an die Statistiksysteme der
Liga. Seit dem Saisonstart am **27. August 2026** läuft das System im
Produktivbetrieb der **Opel Handball-Bundesliga**.

## Wie es funktioniert

| Schritt | Was passiert |
|---|---|
| **1. Daten** | Positionsdaten aus dem Hallen-Trackingsystem und der offizielle Spielverlauf der Liga werden auf der Spieluhr zusammengeführt. |
| **2. Würfe** | Erkannte Wurfereignisse werden gegen den offiziellen Spielverlauf geprüft und Werfer, Torhüter, Spielstand und Spielzeit zugeordnet. |
| **3. Modell** | Ein über mehrere Saisons trainiertes Modell bewertet jede Wurfsituation: xG je Wurf, xS je Torhüter. |
| **4. Qualität** | Ausgeliefert wird nur, was eine ausreichende Datenabdeckung erreicht. Partien mit Lücken in den Trackingdaten werden nicht veröffentlicht. |
| **5. Auslieferung** | Freigegebene Werte gehen zur Halbzeit und nach Spielende automatisch an die Statistikplattform der Liga. |

Betrieb und Datenhaltung finden ausschließlich in deutschen Rechenzentren
statt.

## Repositories

Die produktiven Repositories dieser Organisation sind **privat**, da sie
Betriebsgeheimnisse und Kundendaten berühren. Öffentlich einsehbar ist der
Quelltext der Website.

| | |
|---|---|
| **BieLeMetrics-Website** | Quelltext von bielemetrics.de |
| BieLeMetrics-HBL-Live *(privat)* | Live-Runtime: Datenaufnahme, Zuordnung, Auslieferung, Betriebs-Dashboard |
| BieLeMetrics-HBL *(privat)* | ETL-Strecke, Modelltraining, Auswertungen |
| BieLeMetrics-HBL-infra-common *(privat)* | Infrastruktur als Code |
| BieLeMetrics-HBL-Documentation *(privat)* | Betriebs- und Produktdokumentation |

## Forschungsgrundlage

Das Verfahren stammt aus der Forschung an der Universität Bielefeld und wird
von **Michael Adams** (Technik und Betrieb) und **Alexander David** (Modell und
wissenschaftliche Begleitung) gemeinsam weiterentwickelt.

- Adams, M., David, A., Hesse, M., Rückert, U. (2023).
  *Expected Goals Prediction in Professional Handball using Synchronized Event
  and Positional Data.* MMSports '23, ACM.
  [doi:10.1145/3606038.3616152](https://doi.org/10.1145/3606038.3616152)
- Adams, M. (2023). *A Multimodal System for Automatic Player Tracking in
  Indoor Sports.* Dissertation, Universität Bielefeld.
  [doi:10.4119/unibi/2983118](https://doi.org/10.4119/unibi/2983118)

## Kontakt

Michael Adams · Bielefeld ·
[michael@ad4ms.de](mailto:michael@ad4ms.de) ·
[bielemetrics.de](https://bielemetrics.de) ·
[Impressum](https://bielemetrics.de/impressum.html)

---

<details>
<summary><b>English summary</b></summary>

BieLeMetrics computes **expected goals (xG)** and **expected saves (xS)** for
professional handball. Shot probabilities are derived live from synchronized
positional and event data, quality-gated on tracking coverage, and delivered
automatically to the league's statistics platform. The system has been running
in production for Germany's Opel Handball-Bundesliga since the start of the
2026/27 season. All processing and storage happen in German data centres.

The method originates from research at Bielefeld University
([MMSports '23](https://doi.org/10.1145/3606038.3616152)). Production
repositories are private; the website source is public.

</details>
