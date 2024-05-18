---
title: Ad-hoc-Analysen von Anlagendaten
description: 'Erfahren Sie, wie Sie den Datenanalysemodus verwenden, um Anlagendaten zu analysieren.'
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '5604, 20'
ms.date: 05/02/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Ad-hoc-Analysen von Anlagendaten

In diesem Artikel wird erklärt, wie Sie das Feature **Datenanalyse** zum Analysieren von Anlagendaten direkt von Listenseiten und Abfragen aus verwenden. Sie müssen keinen Bericht ausführen und nicht zu einer anderen Anwendung wie beispielsweise Excel wechseln. Das Feature bietet eine interaktive und vielseitige Möglichkeit, Daten zu berechnen, zusammenzufassen und zu untersuchen. Anstatt Berichte mit Optionen und Filtern auszuführen, können Sie mehrere Registerkarten hinzufügen, die unterschiedliche Aufgaben oder Ansichten der Daten darstellen. Einige Beispiele sind „Aktiva gesamt“, „Abschreibungen im Zeitverlauf“ und jede andere Ansicht, die Sie sich vorstellen können. Weitere Informationen zur Verwendung des Features **Datenanalyse** finden Sie unter [Listen- und Abfragedaten mit dem Analysemodus analysieren](analysis-mode.md).

Nutzen Sie die folgenden Listenseiten um mit der Ad-hoc-Analyse von Anlagenprozessen zu beginnen:

- [Anlagenposten](https://businesscentral.dynamics.com/?page=5604)
- [Sachposten](https://businesscentral.dynamics.com/?page=20)

## Szenarien für die Ad-hoc-Analyse von Anlagendaten

Nutzen Sie das Feature **Datenanalyse** zum schnellen Faktencheck und zur Ad-hoc-Analyse:

- Wenn Sie keinen Bericht ausführen möchten.
- Wenn für Ihren speziellen Bedarf kein Bericht vorhanden ist.
- Wenn Sie schnell iterieren möchten, um sich einen guten Überblick über einen Teil Ihres Unternehmens zu verschaffen.

Die folgenden Abschnitte enthalten Beispiele für Anlagenszenarien in [!INCLUDE [prod_short](includes/prod_short.md)].

| Region | An... | Öffnen Sie diese Seite im Analysemodus | Diese Felder verwenden |
| ---- | ----- | ------------------------------- |------------------- |
| [Anlagen (aktueller Wert)](#example-fixed-assets-current-value) | Verfolgen Sie den Wert von Anlagen nach und zwar sowohl über alle Anlagen hinweg als auch für einen einzelne. | [Anlagenposten](https://businesscentral.dynamics.com/?page=5604) | **Afa-Buch**, **Anlagennr.**, **Anlagenbuchungsdatum**, **Anlagenbuchungsart** und **Betrag** |
|[Beispiel: Abschreibungen auf Anlagen im Zeitverlauf](#example-fixed-asset-depreciations-over-time) | Verfolgen Sie Abschreibungen im Zeitverlauf nach und zwar sowohl über alle Anlagen hinweg als auch für einen einzelne. | [Anlagenposten](https://businesscentral.dynamics.com/?page=5604) | **Afa-Buch**, **Anlagennr.**, **Anlagenbuchungsjahr**, **Anlagenbuchungsmonat**, **Betrag** und **Anlagenbuchungsart** |

### Beispiel: aktueller Wert von Anlagen

Um den Wert einer oder mehrerer Anlagen nachzuverfolgen, gehen Sie wie folgt vor:

1. Öffnen Sie die Liste [Anlagenposten](https://businesscentral.dynamics.com/?page=5604) und wählen Sie :::image type="content" source="media/analysis-mode-icon.png" alt-text="Analysemodus eingeben."::: um den Analysemodus einzuschalten.
1. Gehen Sie zum Menü **Spalten** und entfernen Sie alle Spalten (wählen Sie das Kästchen rechts neben dem Feld **Suchen** aus).
1. Ziehen Sie die Felder **Afa-Buch** und **Anlagennr.** in den Bereich **Zeilengruppen**.
1. Wählen Sie die Felder **Anlagenbuchungsdatum** und **Anlagenbuchungsart** aus.
1. Ziehen Sie das Feld **Menge** in den Bereich **Werte**.
1. Benennen Sie Ihre Analyseregisterkarte in **Anlagenübersicht – Wert** oder in etwas anderes um, das diese Analyse beschreibt.

Das folgende Bild zeigt das Ergebnis dieser Schritte.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png" alt-text="Beispiel für die Durchführung einer Datenanalyse auf der Seite „Anlagenposten“, um sich den Wert einer Anlage anzeigen zu lassen." lightbox="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png":::

### Beispiel: Abschreibungen auf Anlagen im Zeitverlauf

Um die Abschreibung für eine oder mehrere Anlagen nachzuverfolgen, gehen Sie wie folgt vor:

1. Öffnen Sie die Liste [Anlagenposten](https://businesscentral.dynamics.com/?page=5604) und wählen Sie :::image type="content" source="media/analysis-mode-icon.png" alt-text="Analysemodus eingeben."::: um den Analysemodus einzuschalten.
1. Gehen Sie zum Menü **Spalten** und entfernen Sie alle Spalten (wählen Sie das Kästchen rechts neben dem Feld **Suchen** aus).
1. Aktivieren Sie den Schalter **Pivot**-Modus (rechts über dem Feld **Suchen**).
1. Ziehen Sie die Felder **Afa-Buch** und **Anlagennr.** in den Bereich **Zeilengruppen**.
1. Ziehen Sie die Felder **Anlagenbuchungsjahr** und **Anlagenbuchungsmonat** in den Bereich **Spaltenbeschriftungen**.
1. Ziehen Sie das Feld **Menge** in den Bereich **Werte**.
1. Wählen Sie im Filterfeld **Anlagenbuchungsart** die Option **Abschreibung** aus.
1. Benennen Sie Ihre Analyseregisterkarte in **Abschreibung im Zeitverlauf** oder in etwas anderes um, das diese Analyse beschreibt.

Das folgende Bild zeigt das Ergebnis dieser Schritte.

:::image type="content" source="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png" alt-text="Beispiel für die Durchführung einer Datenanalyse auf der Seite „Anlagenposten“, um sich die Abschreibung im Zeitverlauf anzeigen zu lassen." lightbox="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png":::

## Datengrundlage für Ad-hoc-Analysen zu Anlagen

Wenn Sie Anlagen-Buch.-Blätter buchen, erstellt [!INCLUDE [prod_short](includes/prod_short.md)] Posten in der Tabelle **Anlagenposten**. Deshalb werden allgemeine Ad-hoc-Anlagenanalysen normalerweise auf der Seite [Anlagenposten](https://businesscentral.dynamics.com/?page=5604) durchgeführt.

## Siehe auch 

[Listen- und Abfragedaten mit dem Analysemodus analysieren](analysis-mode.md)  
[Anlagenanalysen – Übersicht](fa-analytics-overview.md)  
[Analysen, Business Intelligence und Berichterstellung – Übersicht](reports-bi-reporting.md)  
[Anlagen – Übersicht](fa-manage.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]