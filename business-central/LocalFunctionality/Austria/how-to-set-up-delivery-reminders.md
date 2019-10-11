---
title: 'Gewusst wie: Einrichten von Lieferbenachrichtigungen'
description: In Business Central können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7bf8e32a76f7c2647ff7226f81850357880ea3c9
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300283"
---
# <a name="set-up-delivery-reminders"></a>Gewusst wie: Einrichten von Lieferbenachrichtigungen
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen. Um Lieferanmahnungen für Kreditoren zu erstellen, müssen Sie die Stammdaten für die Erstellung von Lieferanmahnungen sowie die Nummernserien für die Lieferanmahnungen auf der Seite **Kreditoren & Einkauf einrichten** einrichten.  

## <a name="to-set-up-delivery-reminders"></a>Gewusst wie: Einrichten von Lieferbenachrichtigungen  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht  suchen") und geben **Kreditoren- und Debitoren-Einrichtung** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Geben Sie im Feld **Standard Lief.-Mahn. Datumsfeld** eine der Optionen an, wie in der folgenden Tabelle beschrieben.  

    |Option|Beschreibung|  
    |----------------------------------|---------------------------------------|  
    |**Gewünschtes Wareneingangsdatum**|Gibt an, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.|  
    |**Zugesagtes Wareneingangsdatum**|Gibt an, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.|  
    |**Erwartetes Wareneingangsdatum**|Gibt an, dass der Datumswert im Feld **Erwartetes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.|  

3.   Füllen Sie zusätzliche Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Beschreibung|  
    |---------------------------------|---------------------------------------|  
    |**Lieferbenachrichtigungsnummern**|Der Nummernseriencode für Lieferanmahnungen.|  
    |**Reg. Lieferbenachrichtigungsnummern**|Der Nummernseriencode für ausgegebene Lieferanmahnungen.|  

4.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="see-also"></a>Siehe auch  
 [Lieferanmahnungen](delivery-reminders.md)   
 [Einrichten von Lieferbenachrichtigungsbestimmungen, Stufen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md)   
 [So werden Lieferbenachrichtigungscodes zu Kreditoren zugewiesen](how-to-assign-delivery-reminder-codes-to-vendors.md)   
 [So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md)
