---
title: 'Gewusst wie: Registrieren von Lieferbenachrichtigungen'
description: "Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrücken, damit Sie die Benachrichtigungen an Kreditoren senden können. Vor dem Ausstellen von Lieferbenachrichtigungen können Sie einen Testbericht drucken."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: edc847e73bcc3fe7d98ce68311fd9ebbdbc5308c
ms.contentlocale: de-at
ms.lasthandoff: 03/22/2018

---
# <a name="issue-delivery-reminders"></a>Lieferbenachrichtigung registrieren
Nachdem Sie Lieferbenachrichtigungen erstellt haben, müssen Sie sie registrieren und ausdrucken, sodass Sie Mahnungen an Kreditoren verschicken können. Vor dem Ausstellen von Lieferbenachrichtigungen können Sie einen Testbericht drucken. Weitere Informationen finden Sie unter [Vorgehensweise: Drucken von Testberichten für  Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md).  

Beim Registrieren der Lieferantenbenachrichtigungen erzeugt die Anwendung Lieferantenbenachrichtigungsposten. Sie können die generierten Posten im Fenster **Lieferanmahnungsposten** ansehen.  

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

Im registrierten Lieferbenachrichtigungskopf-Fenster, können Sie die Lieferbenachrichtigungsposten der ausgewählten Bestellung anzeigen.  

## <a name="see-also"></a>Siehe auch  
 [Lieferanmahnungen](delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen](how-to-generate-delivery-reminders.md)   
 [So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md)
