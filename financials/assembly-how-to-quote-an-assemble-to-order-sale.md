---
title: 'Vorgehensweise: Angebot eines Auftragsmontageverkaufs | Microsoft Docs'
description: "Sie können Montageverwaltung verwenden, um einen Montageartikel auf Anforderung eines Debitors während des Vertriebsprozesses anzupassen."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7602b067e4b3fc99815a581c851138d7cc3ff41e
ms.contentlocale: de-at
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a>Vorgehensweise: Angebot eines Auftragsmontageverkaufs
Sie können Montageverwaltung verwenden, um einen Montageartikel auf Anforderung eines Debitors während des Vertriebsprozesses anzupassen. Weitere Informationen finden Sie unter [Vorgehensweise: Verkaufen von Auftragsmontageartikeln](assembly-how-to-sell-items-assembled-to-order.md)  

Wie beim Verkauf beliebiger Artikel können Sie auch eine Verkaufsangebot für einen angepassten Montageartikel erstellen, bevor Sie dieses in einen Verkaufsauftrag umwandeln. Dieser Prozess beinhaltet einige zusätzliche Schritte, wenn Sie ihn mit dem Erstellen eines regulären Verkaufsangebots vergleichen; er verwendet eine Variation eines verknüpften Montageauftrags, ein Montageangebot.

> [!NOTE]  
>  Wie alle Arten von Angeboten, werden die Mengen in Montageangeboten nicht für die Verfügbarkeit, in der Planung oder für Reservierungen verwendet.  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a>So erstellen Sie ein Verkaufsangebot für einen Auftragsmontageartikel:  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Verkaufsangebot** ein und wählen dann den zugehörigen Link aus.  
2.  Erstellen Sie eine Verkaufsangebotzeile mit einer Zeile für einen Montageartikel. Weitere Informationen finden Sie unter [Vorgehensweise: Angebote erstellen](sales-how-make-offers.md)  
3.  Geben Sie im Feld **Menge für Auftragsmontage** die vollständige Menge ein.

    > [!NOTE]  
    >  Sie sollten keine Teilmenge eingeben. Daher müssen Sie die gleiche Menge eingeben, die Sie im Feld **Menge** auf der Verkaufsangebotzeile eingegeben haben.  

4.  Wählen Sie auf dem Inforegister **Zeilen** **Zeile** aus, wählen Sie **Auftragsmontage**, und klicken Sie anschließend auf **Auftragsmontagezeilen**. Alternativ wählen Sie das Feld **Menge für Auftragsmontage** aus.  
5.  Prüfen und ändern Sie bei Bedarf im Fenster **Auftragsmontagezeilen** die Auftragsmontagezeilen anhand des Angebots, das der Debitor anfragt. Wenn Sie weitere Informationen wünschen, wählen Sie die Aktion **Dokument anzeigen**, um den vollständigen Rahmenangebotsauftrag zu öffnen. Sie können den Inhalt der meisten Felder nicht ändern, und Sie können nicht buchen.  
6.  Wenn Sie die Montageauftragszeilen entsprechend dem Angebot angepasst haben, schließen Sie das Fenster **Auftragsmontagezeilen**, um zum Fenster **Verkaufsangebot** zurückzukehren.  
7.  Wenn der Kunde das Angebot annimmt, erstellen Sie einen Verkaufsauftrag für den angebotenen Montageartikel. Weitere Informationen finden Sie unter [Vorgehensweise: Angebote erstellen](sales-how-make-offers.md) Das verknüpfte Montageangebot und alle eventuellen Anpassungen werden mit dem neuen Verkaufsauftrag verknüpft, um die Montage des/der zu verkaufenden Artikel vorzubereiten.  

## <a name="see-also"></a>Siehe auch  
[Montageverwaltung](assembly-assemble-items.md)  
[Vorgehensweise: Arbeiten mit Stücklisten](inventory-how-work-BOMs.md)  
[Lagerbest](inventory-manage-inventory.md)  
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

