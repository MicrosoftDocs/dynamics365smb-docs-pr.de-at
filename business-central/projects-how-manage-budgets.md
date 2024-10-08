---
title: Budget für ein Projekt einrichten und verwalten
description: 'Beschreibt, wie Sie Ressourcen planen und die Kosten für ein Projekt durch das Einrichten eines Budgets für jedes Projekt prognostizieren und steuern.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'project budget, forecast'
ms.search.form: '1002, 1007'
ms.date: 02/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="manage-project-budgets"></a>Verwalten von Projektbudgets

Jedes Projekt kann mit einem Budget versehen werden. Das Budget dient zum Planen der Ressourcen, die einem Projekt zugeordnet werden. Dabei kann es sich entweder um ein allgemeines Budget mit nur wenigen Posten oder um ein komplexeres Budget mit einer Vielzahl von Posten handeln, die in verschiedene Aktivitätsstufen unterteilt sind. Mithilfe eines Budgets können die geplanten Beträge mit dem tatsächlichen Verbrauch verglichen werden, der im Buch.-Blatt des Projekts erfasst ist. Durch Überwachung des tatsächlichen Verbrauchs im Vergleich zu einem Budget können sie ein laufendes Projekt kontrollieren und bei späteren Projekten zu einer höheren Qualität beitragen, da sich dadurch die Gefahr unterschätzter Kosten verringert.

Nachfolgend wird beschrieben, wie Sie budgetierte Kosten während der Planung schätzen. Informationen zur Erfassung der budgetierten versus aktueller Preise und Kosten im Projekt finden Sie unter [Erfassen des Verbrauchs für Projekte](projects-how-record-job-usage.md).  

## <a name="to-estimate-the-budgeted-costs-for-a-project"></a><a name="JobBudgetCosts"></a>Die budgetierten Kosten für ein Projekt schätzen

Wenn ein Debitor den Preis eines Projekts erfahren möchte, das auf Grundlage des Verbrauchs fakturiert wird, müssen Sie die budgetierten Einstandspreise für das Projekt ermitteln. Verwenden Sie dazu die Seite **Projektaufgabenzeilen**.

1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](media/ui-search/search_small.png "Tell me-Funktion") und geben Sie **Projekte** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Öffnen Sie ein entsprechendes Projekt.
3. Wählen Sie eine Aufgabenzeile unter Buchung aus und wählen Sie dann die Aktion **Projektplanungszeile**.
4. Füllen Sie die Felder in einer neuen Zeile wie erforderlich aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Für das Feld **Linienart** geben Sie die folgenden Informationen in die Felder ein:  

| Zeilenart | Description |
| --- | --- |
| **Sowohl budgetiert und verrechenbar** |Bei den in der Planungszeile eingegebenen Beträgen für Kosten und Preise handelt es sich um den budgetierten Einstandspreis für diese bestimmte Planungszeile. Der Preisbetrag wird fakturiert. |
| **Budget** |Die Nutzung wird dem Kunden nicht in Rechnung gestellt. Die Nutzung wird nicht in eine Rechnung übertragen, sondern zur Berechnung des WIP verwendet. |
| **Fakturierbar** |Die Nutzung wird dem Kunden in Rechnung gestellt. Der Verbrauch wird auf die Rechnung übertragen, und basiert auf der Menge, die in dem **In Rechnung zu übertrag. Menge angegeben** ist. |

> [!NOTE]  
> Das Feld **Geplantes Lieferdatum** für die Planungszeile enthält das Datum, wann der Verbrauch, der mit der Planungszeile verknüpft wird, erwartungsgemäß abgeschlossen. Es ist ebenfalls das Datum, an dem die Planungszeile in eine Verkaufsrechnung übertragen und gebucht wird. <br /><br /> Auf der zugrunde liegenden Projektaufgabe auf der Seite **Projektkarte** enthalten die Felder **Startdatum** und **Enddatum** jeweils die Werte für **Geplantes Lieferdatum** der frühesten spätesten und Projektplanzeilen auf der entsprechenden **Projektplanzeilen**-Seite.

> [!NOTE]  
> Geben Sie die Menge für das Feld **Planungszeile** ein. Alle Angaben zu Einstands- und Verkaufsbeträgen werden nun berechnet und für diese Planungszeile eingetragen. Sie können nun jederzeit bearbeitet werden.

Auf der Seite **Projektkarte** können Sie nun eine Zusammenfassung mit budgetiertem Einstandsbetrag, budgetiertem Verkaufsbetrag, fakturierbaren Kosten und fakturierbarem Preis für jede Aufgabe anzeigen.

Informationen zur Erfassung der budgetierten versus aktueller Preise und Kosten im Projekt finden Sie unter [Erfassen des Verbrauchs für Projekte](projects-how-record-job-usage.md).

## <a name="see-also"></a>Siehe auch

[Projektmanagement](projects-manage-projects.md)  
[Finanzen](finance.md)  
[Einkauf](purchasing-manage-purchasing.md)  
[Verkauf](sales-manage-sales.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
