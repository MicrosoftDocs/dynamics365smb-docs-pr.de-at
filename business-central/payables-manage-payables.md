---
title: Übersicht über die Aufgaben zum Verwalten von Kreditorenkonten
description: 'Gliedert Aufgaben, um Debitoren zu verwalten, beispielsweise zahlende Gläubiger oder ausgehende Zahlungen an Buch-Posten, um Rechnungen oder Gutschriften zu schließen.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: overview
ms.devlang: al
ms.search.keywords: 'vendor payment, creditor, debt, balance due, AP'
ms.search.form: '161, 254, 256, 347, 574, 599, 9002'
ms.date: 07/12/2024
ms.service: dynamics-365-business-central
---

# <a name="managing-payables"></a>Verwalten von Verbindlichkeiten

Ein großer Teil der Verwaltung großer aus das Wareneinkaufskonto zahlt Ihre Kreditoren oder erstattet Mitarbeiter für Ausgaben zurück. Sie können Funktionalität verwenden, um die Seite **Zahlung Buch.-Blatt** automatisch mit Zahlungszeilen für fällige Einkaufsrechnungen auszufüllen. Um die entsprechenden Banktransaktionen schnell auszuführen, können Sie mehrere Zahlungsausgangs Buch.-Blattzeilen in eine Datei exportieren, die Sie dann für Ihre Bank für die Verarbeitung hochladen. Sie können Zahlungen auch mit Scheck leisten inkl. der Möglichkeit, Schecks als elektronisches Zahlungsmittel zu senden.

Eine weitere typische Aufgabe ist es, ausgehenden Zahlungen dem zugehörigen Debitor bzw. einem Kreditorenposten zuzuordnen, um die entsprechenden Einkaufsrechnungen oder Einkaufsgutschriften zu schließen, wenn sie bezahlt sind. Diese Aufgabe können Sie dann auf der Seite **Zahlungs-Abstimmungs-Buch.-Blatt** ausführen, indem Sie eine Bankkontoauszugsdatei importieren, um die Zahlungen schnell zu erfassen. Die Zahlungen werden angewendet, um Debitoren- oder Kreditorenposten zu öffnen, indem passender Zahlungstext und Zahlungsinformationen verknüpft werden. Es gibt verschiedene Arten, die Übereinstimmungen zu prüfen und zu ändern, bevor Sie das Buch.-Blatt buchen. Sie können die offenen Bankkontoposten für ausgeglichenen Posten schließen, wenn Sie das Buch.-Blatt buchen. Das bedeutet, dass das Bankkonto automatisch abgestimmt wird, wenn alle Zahlungen ausgeglichen werden.

Alternativ können Sie ausgehende Zahlungen auf der Seite **Zahlungsausgangs Buch.-Blatt** oder aus den zugehörigen Kreditorenposten manuell ausgleichen.

Die folgende Tabelle enthält eine Abfolge von Aufgaben sowie Links zu den Kreditoren, in denen diese Artikel erläutert werden.

| An | Siehe |
| --- | --- |
| Generieren von Fälligkeitsdatum oder Kreditorenzahlungen oder Mitarbeitervergütungen, bereiten Sie Scheckzahlungen vor und exportieren sie Zahlungen beim Buchen an eine Bank. |[Zahlungen vornehmen](payables-make-payments.md) |
| Gleichen Sie Kreditorenzahlungen automatisch für unbezahlte Einkaufsrechnungen aus, indem Sie eine Bankkontoauszugsdatei importieren. |[Zahlungen automatisch vornehmen und Bankkonten abstimmen](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Gleichen Sie Kreditorenzahlungen für unbezahlten Einkaufsrechnungen manuell aus. |[Abstimmen von Kreditorenzahlungen mit dem Zahlungsjournal oder aus Kreditorenposten](payables-how-apply-purchase-transactions-manually.md) |
|Um eine korrekte Bewertung sicherzustellen, müssen Ihre Lagerartikel Kosten wie Fracht, Versicherung, Umlagerung und Transport enthalten, die beim Kauf oder Verkauf entstehen.|[Verwenden von Artikelzuschlägen für zusätzliche Kosten](payables-how-assign-item-charges.md)|
|Erstatten Sie Mitarbeitern persönliche Ausgaben für die Geschäftsaktivitäten zurück, indem Sie Zahlung zu dem Bankkonto vornehmen.|[Ausgaben der Beschäftigten aufzeichnen und erstatten](finance-how-record-reimburse-employee-expenses.md)|

## <a name="see-also"></a>Siehe auch
[Einkauf](purchasing-manage-purchasing.md)    
[Verwaltung von Forderungen](receivables-manage-receivables.md)    
[Verwenden Sie Artikelgebühren, um zusätzliche Handelskosten zu berücksichtigen](payables-how-assign-item-charges.md)    
[Allgemeine Geschäftsfunktionen](ui-across-business-areas.md)    
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]
