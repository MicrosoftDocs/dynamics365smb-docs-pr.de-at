---
title: 'Gewusst wie: Registrieren von Lieferbenachrichtigungen'
description: "Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrücken, damit Sie die Benachrichtigungen an Kreditoren senden können. Vor der Registrierung der Lieferbenachrichtigungen können Sie einen Testbericht drucken."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: b5a6e59cddd7ac1d22af73f40cd83f2a4a9860d9
ms.contentlocale: de-at
ms.lasthandoff: 03/22/2018

---
# <a name="issue-delivery-reminders"></a>Lieferbenachrichtigung registrieren
Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrücken, damit Sie die Benachrichtigungen an Kreditoren senden können. Vor dem Ausstellen von Lieferbenachrichtigungen können Sie einen Testbericht drucken. Weitere Informationen finden Sie unter [Vorgehensweise: Drucken von Testberichten für  Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md).  

Beim Registrieren der Lieferbenachrichtigungen werden Lieferanmahnungsposten erstellt. Sie können die generierten Posten im Fenster **Lieferanmahnungsposten** ansehen.  

## <a name="to-issue-delivery-reminders"></a>So registrieren Sie Lieferbenachrichtigungen  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") , geben Sie **Lieferbenachrichtigung** ein, und wählen Sie dann den zugehörigen Link.  
2.  Wählen Sie im Fenster **Lieferbenachrichtigung** die Lieferbenachrichtigung, die Sie registrieren möchten, und wählen Sie dann die Aktion **Bearbeiten**.  
3.  Wählen Sie die Aktion **Registrieren**.  
4.  Füllen Sie im Fenster **Lieferbenachrichtigung registrieren** auf dem Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Drucken**|Wählen Sie die zu druckenden Lieferbenachrichtigungen aus, nachdem sie registriert wurden.|  
    |**Buchungsdatum ersetzen**|Geben Sie an, dass das vorhandene Buchungsdatum für die Lieferbenachrichtigung ersetzt werden soll.|  
    |**Buchungsdatum**|Gibt das Buchungsdatum der Lieferbenachrichtigung an.<br /><br /> Dieses Buchungsdatum wird für alle Lieferbenachrichtigungen verwendet, wenn Sie das Kontrollkästchen **Buchungsdatum ersetzen** aktiviert haben. Wenn das Kontrollkästchen **Buchungsdatum ersetzen** deaktiviert ist, wird dieses Datum nur für die Lieferbenachrichtigungen verwendet, für die kein Buchungsdatum verfügbar ist.|  

5.  Wählen Sie optional auf dem Inforegister **Lieferbenachrichtigungskopf** die gewünschten Filter aus.  

    > [!NOTE]  
    >  Sie können die Filter entfernen und alle Lieferbenachrichtigungen gleichzeitig übermitteln.  

6.  Wählen Sie die Schaltfläche **OK** aus.  

Sie können die registrierten Lieferbenachrichtigungen im Fenster **Reg. Lieferbenachrichtigung** betrachten. Wenn Sie möchten, können Sie jetzt eine Lieferbenachrichtigung drucken.  

## <a name="to-view-delivery-reminder-ledger-entries"></a>So zeigen Sie die Lieferanmahnungsposten an  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Gebuchte Aufträge** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Bestellung aus, für die Sie den Benachrichtigungsstatus anzeigen möchten, und wählen Sie dann die Aktion **Bearbeiten**.  
3.  Wählen Sie die Aktion **Lieferanmahnungsposten**.  

Im Fenster „Lieferanmahnungsposten” können Sie die Lieferbenachrichtigungsposten für die ausgewählte Bestellung betrachten.  

## <a name="see-also"></a>Siehe auch  
 [Lieferanmahnungen](delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen](how-to-generate-delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md)

