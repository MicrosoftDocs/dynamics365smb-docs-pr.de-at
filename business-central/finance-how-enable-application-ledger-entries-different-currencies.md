---
title: Ausgleichen von Posten in unterschiedlichen Währungen| Microsoft Docs
description: Wenn Sie an einen Debitor in einer Währung verkaufen, die Zahlung jedoch in einer anderen Währung erfolgt, kann die Rechnung mit der Zahlung ausgeglichen werden.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 564ac8edfb21573e310a3be3eaa22060d84bef22
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4750922"
---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a>Anwendung von Kreditorenposten in unterschiedlichen Währungen aktivieren
Falls Sie Einkäufe von einem Kreditor in einer Währung tätigen und die Zahlung in einer anderen Währung leisten, können Sie die Zahlung mit dem Einkauf ausgleichen.

Wenn Sie entsprechend an einen Debitor in einer Währung verkaufen und die Zahlung in einer anderen Währung erhalten, können Sie die Zahlung mit der Verkaufsrechnung ausgleichen.

Im Folgenden wird beschrieben, wie dies für Kreditorenposten auf der Seite **Kreditoren & Einkauf Einrichtung** eingerichtet wird. Die Einrichtung für Debitorenposten auf der Seite **Debitoren & Verkauf Einrichtung** ist ähnlich.

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>So aktivieren Sie den Ausgleich von Kreditorenposten in unterschiedlichen Währungen
1. Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Einrichten von Einkäufen und Verbindlichkeiten** ein, und wählen Sie dann den zugehörigen Link aus.
2. Wählen Sie im Feld **Währungsausgleich** eine der folgenden Optionen.

| Option | Beschreibung |
| --- | --- |
| Keine |Ausgleich zwischen Währungen ist nicht zugelassen. |
| EWU |Ausgleich zwischen EWU-Währungen ist zugelassen. |
| Alle |Ausgleich zwischen allen Währungen ist zugelassen. |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a>So richten Sie Sachkonten für Rundungsdifferenzen beim Währungsausgleich ein  
Wenn Sie Posten in unterschiedlichen Währungen ausgleichen, müssen Sie die Sachkonten einrichten, auf die Sie die Rundungsdifferenzen buchen möchten.  

> [!NOTE]  
>  Sie müssen die Sachkonten einrichten, bevor Sie die Aufgabe abschließen. Weitere Informationen finden Sie unter [Verständis der Fibu und des Kontoplans](finance-general-ledger.md).

1. Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell Me-Funktion") aus, geben Sie **Debitorenbuchungsgruppen** ein und wählen Sie dann den entsprechenden Link.  
2. Geben Sie in die Felder **Währungsausgl. Rund.-Sollkto.** und **Währungsausgl. Rund.-Habenkto.** die entsprechenden Sachkonten ein, um Rundungsdifferenzen zu buchen.  
3. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Kreditorenbuchungsgruppen** ein, und wählen Sie dann den entsprechenden Link.  
4. Geben Sie in die Felder **Währungsausgl. Rund.-Sollkto.** und **Währungsausgl. Rund.-Habenkto.** die entsprechenden Sachkonten ein, um Rundungsdifferenzen zu buchen.  

## <a name="see-also"></a>Siehe auch
[Verwalten von Verbindlichkeiten|](payables-manage-payables.md)  
[Verwalten von Forderungen](receivables-manage-receivables.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]