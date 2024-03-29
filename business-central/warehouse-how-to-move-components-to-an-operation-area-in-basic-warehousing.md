---
title: So verschieben Sie Komponenten in einen Arbeitsgangbereich in Basis-Lagerkonfigurationen
description: Wenn die Arbeitsgänge, die den Artikel verarbeiten, an Ihrem Lagerort stattfinden, müssen Sie möglicherweise Artikel zwischen internen Lagerplätzen umlagern, um auf interne Herkunftsbelege, wie Produktions-, Montage- oder Serviceaufträge am Lagerort zu reagieren.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 7351, 7382, 9330
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: da2f937c50e5634a5f4e3abe6d1eae9064916f52
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/31/2022
ms.locfileid: "8513280"
---
# <a name="move-components-to-an-operation-area-in-basic-warehouse-configurations"></a>So verschieben Sie Komponenten in einen Arbeitsgangbereich in Basis-Lagerkonfigurationen
Wenn die Arbeitsgänge, die den Artikel verarbeiten, an Ihrem Lagerort stattfinden, müssen Sie möglicherweise Artikel zwischen internen Lagerplätzen umlagern, um auf interne Herkunftsbelege, wie Produktions-, Montage- oder Serviceaufträge am Lagerort zu reagieren.  

> [!NOTE]  
>  Weitere Informationen zum Umlagern von Artikeln ohne Herkunftsbelege finden Sie unter Interne Umlagerung.  

In erweiterten Lagerkonfigurationen, in denen Lagerplätze das Einrichtungsfeld **Gesteuerte Einlag. u. Kommiss.** verwenden, können Sie die Seite **Lagerplatzumlagerungsarbeitsblatt** verwenden, um die Artikel zwischen Lagerplätzen umzulagern. Weitere Informationen finden Sie unter [Vorgehensweise: Umlagerung von Artikeln in erweiterten Lagerkonfigurationen](warehouse-how-to-move-items-in-advanced-warehousing.md).  

In den Basislagerkonfigurationen, in denen Lagerplätze das Einrichtungsfeld **Lagerplatz notwendig** und das Einrichtungsfeld **Kommissionierung erforderlich** verwenden , können Umlagerungen von Artikeln an interne Vorgangsbereiche basierend auf internen Herkunftsbelegen auf die folgenden Arten gebucht werden:  

-   Auf der Seite **Lagerbewegung**.  
-   Mit der Seite **Lagerkommissionierung**.  

> [!NOTE]  
>  Lagerkommissionierungen buchen auch negative Artikelposten als Verbrauch und werden nur für Produktionskomponenten unterstützt. Weitere Informationen finden Sie auf der Seite Arbeitsblatt Auslieferung.  

Ausführliche Informationen zu Lagerbewegungen finden Sie auf der Seite Lagerbewegung.  

Zwei verschiedene Rollen können die erste Lagerbewegung erstellen. Ein Montagearbeiter kann diese beispielsweise aus einem freigegebenen Montageauftrag erstellen, sodass diese in der Liste der offenen Arbeiten des Lagermitarbeiters angezeigt wird. Um eine Lagerbewegung für Montageauftragszeilen zu erstellen, die bereit sind, dass Komponenten in ihre festgelegten Lagerplätze umgelagert werden, verwendet der Montagearbeiter die Funktion **Lagerbewegung erstellen**.  

Alternativ kann ein Lagermitarbeiter diese erstellen, indem er auf den freigegebenen Montageauftrag verweist. Dies wird im folgender Verfahren beschrieben.  

> [!NOTE]  
>  Wenn die Umlagerung für einen Montageauftrag erfolgt, in dem der Artikel für einen Auftrag montiert wird, dann können Sie festlegen, dass der Lagerbewegungsbeleg automatische erstellt wird, wenn Sie den Lagerkommissionierungsbeleg für den fertigen Montageartikel erstellen, der die Lieferung bucht. Um dies einzurichten, wählen Sie das Feld **Umlagerungen automatisch erstellen** auf der Seite **Montageeinrichtung** aus  
>   
>  Weitere Informationen zu Montageaufträgen und Basis-Lagerkonfigurationen finden Sie unter [Verarbeiten von Auftragsmontageartikeln mit Lagerkommissionierungen](warehouse-how-to-pick-for-production.md#handling-assemble-to-order-items-with-inventory-picks).  

Im folgenden Verfahren wird beschrieben, wie eine Lagerbewegung aus der Seite **Lagerbewegung** durch das Verweisen auf einen freigegebenen Montageauftrag als Herkunftsbeleg erstellt wird. Dieser Vorgang ist derselbe, wenn Sie Komponenten für Fertigungsaufträge und Serviceaufträge umlagern.  

## <a name="to-move-components-to-an-operation-area-in-basic-warehouse-configurations"></a>So lagern Sie Komponenten in einen Arbeitsgangbereich in Basis-Lagerkonfigurationen um  
1.  Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](media/ui-search/search_small.png "Tell me-Funktion") Symbol. Geben Sie **Lagerbewegungen** ein und wählen Sie den entsprechenden Link.  
2.  Füllen Sie auf dem Inforegister **Allgemein** das Feld **Nr.** aus. Feld Sie können die EINGABETASTE betätigen, um in den Nummernserien eine Auswahl zu treffen.  
3.  Geben Sie im Feld **Lagerortcode** den Lagerort ein, an dem die Umlagerung stattfindet.  
4.  Wählen Sie die **Herkunftsbelege holen** Aktion aus. Füllen Sie alternativ das Feld **Herkunftsbeleg** aus, und klicken Sie anschließend auf die Schaltfläche **AssistEdit** im Feld **Herkunftsnr.**.  
5.  Wählen Sie auf der Seite **Herkunftsbelege** den Montageauftrag aus, für den Sie Komponenten umlagern möchten, und klicken Sie anschließend auf die Schaltfläche **OK**.  

    Für alle erforderlichen Komponenten, die umgelagert werden können, werden auf der Seite **Lagerbewegungen** eine Entnahme- und eine Einlagerungszeile generiert. Alle Felder mit Ausnahme des Felds **Bewegungsmenge** werden entsprechend den Herkunftsbelegzeilen vorbelegt. Das Feld **Bewegungsmenge** weist Null aus, bis Sie die Menge angeben, die Sie tatsächlich umgelagert haben.  

    Sie können den Lagerplatzcode in einer Entnahmezeile aber nur entsprechend der Verfügbarkeit ändern. Wenn Sie in einer Entnahmezeile die Schaltfläche **AssistEdit** im Feld **Lagerplatzcode** auswählen, wird die Seite **Lagerplatzinhalt** geöffnet und zeigt nur Lagerplätze an, an denen die Komponente verfügbar ist.  

    Sie können den Lagerplatzcode in einer Einlagerungszeile nicht ändern. Nur der Lagerplatzcode, der in der Komponentenzeile des Herkunftsbelegs definiert ist, wird angenommen. Dies unterstützt das Prinzip, dass die Rolle, die eine Komponente anfordert, hier ein Montagearbeiter, weiß, wo die Komponente platziert werden muss. Wenn Sie die Komponenten an einem anderen Lagerplatz einlagern möchten, müssen Sie zuerst den Lagerplatzcode in der Komponentenzeile ändern und die Lagerbewegungszeilen dann neu erstellen.  
6.  Geben Sie im Feld **Bewegungsmenge** die vollständige oder einen Teil der Menge ein, die Sie tatsächlich umgelagert haben. Die Werte in den Zeilen "Entnahme" und "Einlagerung" müssen gleich sein. Andernfalls kann die Lagerplatzumlagerung nicht gebucht werden.  

    > [!NOTE]  
    >  Wie bei anderen Lageraktivitäten, können Sie die Einlagerungszeile aufteilen, indem Sie die Aktion **Aktionen** und dann die Aktion **Zeile aufteilen** auswählen. In diesem Fall muss die Summe der beiden geteilten Einlagerungszeilen der Menge in der Zeile für die Entnahme entsprechen.  

7.  Wenn Sie bereit sind, die Umlagerungen zu erfassen, die Sie durchgeführt haben, wählen Sie die Aktion **Lagerbestandsumlagerung registrieren**.  

    Die Lagerplatzposten werden erstellt und zeigen an, dass die Komponenten jetzt an den Lagerplätzen vorhanden sind, die in den Montageauftragszeilen angegeben sind.  

    > [!NOTE]  
    >  Anders als beim Umlagern von Komponenten mit einer Lagerkommissionierung, wird Verbrauch nicht gebucht, wenn Sie eine Lagerbewegung erfassen. Dieser Schritt muss separat ausgeführt werden, indem Istmeldung und Verbrauch des Montageauftrags gebucht werden. Weitere Informationen finden Sie unter Montageauftrag.  

## <a name="see-also"></a>Siehe auch  
[Logistik](warehouse-manage-warehouse.md)  
[Lagerbesttand](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]