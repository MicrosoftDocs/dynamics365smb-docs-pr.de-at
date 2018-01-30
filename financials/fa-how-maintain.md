---
title: Anlagen verwalten | Microsoft Docs
description: "Sie müssen einen Instandhaltungsbericht aller Reparaturen und Services einer Anlage führen."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 71210a9acbd196581aa4397264b462728007e5e8
ms.contentlocale: de-at
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-maintain-fixed-assets"></a>So geht's: Anlagen aktualisieren
Wartungsausgaben sind periodische Kosten, die dem Werterhalt von Anlagen dienen. Im Gegensatz zu Kapitalerhöhungen wird der Wert dabei nicht erhöht.

Sie können den Service und die Wartung Ihrer Anlagen erfassen, sodass Ihnen jederzeit aktuelle Daten zur Wartung Ihrer Anlagen zur Verfügung stehen. Bei jedem Service, der für eine Anlage durchgeführt wird, werden die entsprechenden Daten wie Servicedatum, Kreditorennummer und Telefonnummer der Wartungsfirma erfasst. Die Registrierung der Wartung erfolgt auf der Anlagenkarte der jeweiligen Anlage.

Die Indexierung wird verwendet, um die Werte allgemeinen Preisänderungen anzupassen. Die Stapelverarbeitung **Anlagen indexieren** kann verwendet werden, um Wartungskosten neu zu berechnen.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>So erfassen Sie Wartungsarbeiten in einer Anlage
Jedes Mal, wenn eine Wartung ausgeführt wurde, wie z.B. ein Servicebesuch, können Sie diese für die entsprechende Anlage im Fenster **Wartungsregistrierung** erfassen.  

1. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Wählen Sie die Anlage aus, für die Sie die Wartung übernehmen möchten und wählen Sie dann die Aktion **Wartungsregistrierung** aus.
3. Füllen Sie im Fenster **Wartungsregistrierung** die Felder nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>So buchen Sie Wartungskosten aus einem Anlagen Fibu Buch.-Blatt
1. Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen]das Symbol (media/ui-search/search_small.png "")Nach Seite oder Bericht suchen und geben **AfA-Buchliste** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Wählen Sie das AfA-Buch aus, das der Anlage zugewiesen ist, und wählen Sie dann die Aktion **Bearbeiten** aus.
3. Stellen Sie im Fenster **AfA-Buch - Karte** sicher, dass das Kontrollkästchen **Wartung** nicht aktiviert ist. Dadurch ist sichergestellt, dass keine Wartungskosten in der Finanzbuchhaltung gebucht werden.
4. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen G/L-Buchblatt** ein und wählen den zugehörenden Link aus.  
5. Erstellen Sie eine ursprüngliche Buch.-Blattzeile und füllen Sie die notwendigen Felder aus.
6. Wählen Sie im Feld **Anlagenbuchungsart** die **Wartung**.
7. Wählen Sie die Aktion **Anlagengegenkonto einfügen**. Eine zweite Buch.-Blattzeile wird für das Gegenkonto erstellt, das für die Buchung einer Wartung eingerichtet wird.

    > [!NOTE]  
>   Schritt 7 funktioniert nur, wenn Sie Folgendes eingerichtet haben: Im Fenster **Anlagenbuchungsgruppenkarte** der Buchungsgruppe der Anlage enthält das Feld **Kto. Wartung** das Sollkonto im Sachkonto und das Feld **Gegenkto. Wartung** enthält das Sachkonto, auf das die Gegenposten für Zuschreibungen gebucht werden sollen. Weitere Informationen finden Sie im Abschnitt "So richten Sie Anlagenbuchungsgruppen ein" in [So geht's: Allgemeine Anlageninformationen einrichten](fa-how-setup-general.md).
8. Wählen Sie die Aktion **Buchen** aus.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>So führen Sie Folgeaktionen nach Servicebesuchen für Anlagen aus
Sie können den Bericht **Wartung - Nächster Service** drucken, um anzuzeigen, für welche Anlagen ein Servicebesuch geplant ist. Sie können diesen Bericht auch verwenden, wenn Sie das Feld **Nächstes Servicedatum** auf den Anlagenkarten aktualisieren.  

1. Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen]das Symbol (media/ui-search/search_small.png "")Nach Seite oder Bericht suchen und geben **AfA-Buchliste** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Füllen Sie die Felder **Startdatum** und **Enddatum** aus.  
3. Klicken Sie auf die Schaltfläche **Drucken** oder **Vorschau**.

## <a name="to-monitor-maintenance-costs"></a>So prüfen Sie Wartungskosten
Sie können die Wartungskosten einsehen, wenn Sie sich die Statistik einer Anlage anzeigen lassen.  

1. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.
2. Wählen Sie die Anlage aus, für die Sie die Wartungskosten anzeigen möchten und wählen Sie dann die Aktion **AfA-Bücher** aus.
3. Wählen Sie im Fenster **Anlagen-AfA-Bücher** das relevante Anlagen-AfA-Buch aus, und dann die Aktion **Statistik**.
4. Klicken Sie zum Öffnen des Fensters **Anlagenstatistik** auf das Feld **Wartung**.

Das Fenster **Wartungsposten** wird geöffnet und zeigt die Posten an, aus denen sich der Betrag im Feld **Wartung** zusammensetzt.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>So werden Wartungskosten für mehrere Anlagen angezeigt oder gedruckt
In dem Bericht **Wartungsanalyse** können Sie auswählen, ob Sie sich Wartungen basierend auf ein, zwei oder drei Wartungscodes für ein bestimmtes Datum oder ein Datumsintervall anzeigen lassen wollen. Sie können sich eine Gesamtsumme für alle ausgewählten Anlagen oder eine Summe für jede einzelne Anlage anzeigen lassen.

1. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Wartungsanalyse** ein und wählen den zugehörenden Link aus.
2. Füllen Sie die Felder je nach Bedarf aus.
3. Klicken Sie auf die Schaltfläche **Drucken** oder **Vorschau**.

## <a name="to-view-maintenance-ledger-entries"></a>So zeigen Sie Wartungsposten an
Sie können sich ausserdem die Wartungskosten ansehen, wenn Sie sich die Wartungsposten anzeigen lassen.  

1. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.
2. Wählen Sie die Anlage aus, für die Sie die Posten anzeigen möchten und wählen Sie dann die Aktion **AfA-Bücher** aus.
3. Wählen Sie im Fenster **Anlagen-AfA-Bücher** das relevante Anlagen-AfA-Buch aus, und dann die Aktion **Wartungsposten**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>So werden Wartungsposten für mehrere Anlagen angezeigt oder gedruckt
Sie können im Bericht **Wartungsdetails** Wartungsposten für eine oder mehrere Anlagen anzeigen oder drucken.  

1. Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Wartungsanalyse** ein und wählen den zugehörenden Link aus.
2. Füllen Sie die Felder je nach Bedarf aus.
3. Klicken Sie auf die Schaltfläche **Drucken** oder **Vorschau**.

## <a name="see-also"></a>Siehe auch
[Anlagen](fa-manage.md)  
[Anlagen einrichten](fa-setup.md)  
[Finanzen](finance.md)  
[Willkommen bei [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
