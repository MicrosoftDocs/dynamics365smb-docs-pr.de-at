---
title: 'Gewusst wie: Registrieren von Lieferbenachrichtigungen'
description: Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrücken, damit Sie die Benachrichtigungen an Kreditoren senden können. Vor der Registrierung der Lieferbenachrichtigungen können Sie einen Testbericht drucken.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 4be4475a9bce2b0db4820e35d40a0ee2cd1c45d9
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 06/28/2019
ms.locfileid: "1710971"
---
# <a name="issue-delivery-reminders"></a>Lieferbenachrichtigung registrieren
Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrücken, damit Sie die Benachrichtigungen an Kreditoren senden können. Vor dem Ausstellen von Lieferbenachrichtigungen können Sie einen Testbericht drucken. Weitere Informationen finden Sie unter [Vorgehensweise: Drucken von Testberichten für  Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md).  

Beim Registrieren der Lieferbenachrichtigungen werden Lieferanmahnungsposten erstellt. Sie können die generierten Posten auf der Seite **Lieferanmahnungsposten** ansehen.  

## <a name="to-issue-delivery-reminders"></a>So registrieren Sie Lieferbenachrichtigungen  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), geben Sie **Lieferanmahnung** ein, und wählen Sie dann den zugehörigen Link.  
2.  Wählen Sie auf der Seite **Lieferanmahnung** die Lieferanmahnung, die Sie registrieren möchten, und wählen Sie dann die Aktion **Bearbeiten**.  
3.  Wählen Sie die Aktion **Registrieren**.  
4.  Füllen Sie auf der Seite **Lieferanmahnung registrieren** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Drucken**|Wählen Sie die zu druckenden Lieferbenachrichtigungen aus, nachdem sie registriert wurden.|  
    |**Buchungsdatum ersetzen**|Geben Sie an, dass das vorhandene Buchungsdatum für die Lieferbenachrichtigung ersetzt werden soll.|  
    |**Buchungsdatum**|Gibt das Buchungsdatum der Lieferbenachrichtigung an.<br /><br /> Dieses Buchungsdatum wird für alle Lieferbenachrichtigungen verwendet, wenn Sie das Kontrollkästchen **Buchungsdatum ersetzen** aktiviert haben. Wenn das Kontrollkästchen **Buchungsdatum ersetzen** deaktiviert ist, wird dieses Datum nur für die Lieferbenachrichtigungen verwendet, für die kein Buchungsdatum verfügbar ist.|  

5.  Wählen Sie optional auf dem Inforegister **Lieferbenachrichtigungskopf** die gewünschten Filter aus.  

    > [!NOTE]  
    >  Sie können die Filter entfernen und alle Lieferbenachrichtigungen gleichzeitig übermitteln.  

6.  Wählen Sie die Schaltfläche **OK**.  

Sie können die registrierten Lieferanmahnungen auf der Seite **Reg. Lieferanmahnung** betrachten. Wenn Sie möchten, können Sie jetzt eine Lieferbenachrichtigung drucken.  

## <a name="to-view-delivery-reminder-ledger-entries"></a>So zeigen Sie die Lieferanmahnungsposten an  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Gebuchte Aufträge** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Bestellung aus, für die Sie den Benachrichtigungsstatus anzeigen möchten, und wählen Sie dann die Aktion **Bearbeiten**.  
3.  Wählen Sie die Aktion **Lieferanmahnungsposten**.  

Auf der Seite **Lieferanmahnungsposten** können Sie die Lieferanmahnungsposten für die ausgewählte Bestellung betrachten.  

## <a name="see-also"></a>Siehe auch  
 [Lieferanmahnungen](delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen](how-to-generate-delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md)
