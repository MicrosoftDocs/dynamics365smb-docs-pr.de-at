---
title: Lageraktivitäten | Microsoft Docs
description: Nach dem Eingang und vor der Lieferung von Waren finden einige interne Lageraktivitäten statt, um einen effektiven Ablauf im Lager zu gewährleisten und um den Lagerbestand des Unternehmens zu organisieren und zu verwalten.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: eef51c7fe686b9cfa2383930cf7daef3ef3d6f02
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4755884"
---
# <a name="warehouse-management"></a>Logistik
Nach dem Eingang und vor der Lieferung von Waren finden einige interne Lageraktivitäten statt, um einen effektiven Ablauf im Lager zu gewährleisten und um den Lagerbestand des Unternehmens zu organisieren und zu verwalten.

Zu den typischen Lageraktivitäten gehören das Einlagern von Artikeln, das Umlagern von Artikeln in Lagern oder zwischen Lagern und die Kommissionierung von Artikeln für die Montage, Produktion oder Lieferung. Die Montage von Artikeln für Verkäufe oder Lager gilt auch als Lageraktivität, doch diese werden an anderer Stelle behandelt. Weitere Informationen finden Sie unter [Montageverwaltung](assembly-assemble-items.md).  

In großen Lagern können diese unterschiedlichen Aufgaben nach Abteilungen getrennt sein und die Integration kann durch einen gesteuerten Workflow verwaltet werden. In einfacheren Installationen ist der Auftragsfluss weniger formalisiert und die Lageraktivitäten werden mit sogenannten Lagerbestandseinlagerungen und -kommissionierungen durchgeführt. Weitere Informationen über grundlegende und erweiterte Lagerkonfigurationen finden Sie unter [Designdetails: Logistik Übersicht](design-details-warehouse-overview.md).

Bevor Sie Lageraktivitäten ausführen können, müssen Sie das System für die relevante Komplexität der Lagerverarbeitung einrichten. Weitere Informationen finden Sie unter [Lagerortverwaltung einrichten](warehouse-setup-warehouse.md).

Die lagerbezogenen Aufgaben der Zählung, Anpassung und Umbuchung von Artikeln beinhaltet möglicherweise Lageraufgaben, die für Lagerplatzposten ausgeführt werden müssen, bevor sie mit den zugehörigen Artikelposten synchronisiert werden können. Weitere Informationen finden Sie unter [Erfassen, Regulieren und Umbuchen von Lagerbestand](inventory-how-count-adjust-reclassify.md).

 In der folgenden Tabelle wird eine Reihe von Aufgaben mit Verknüpfungen zu den beschriebenen Themen erläutert   

|**Aufgabe**|**Siehe**|  
|------------|-------------|  
|Erfassung des Eingangs (einschließlich des Übereingangs) von Artikeln an Lagerstandorten, entweder nur mit einer Bestellung, bei einfachen Standorteinrichtungen, oder mit einem Lagerschein, im Falle einer halb- oder vollautomatischen Lagerabwicklung am Standort.|[Empfangen von Artikeln](warehouse-how-receive-items.md)|
|Umgehen Sie die Einlagerungs- und Kommissionierungsvorgänge, um einen Artikel direkt vom Wareneingang oder der Fertigung zum Versenden zu beschleunigen.|[Zuordnungselemente](warehouse-how-to-cross-dock-items.md)|    
|Lagern Sie Artikel ein, die bei Einkäufen, Verkaufsrücksendungen, Umlagerungen oder Fertigerzeugnissen eingehen, gemäß dem konfigurierten Lageraktivitätsvorgang ein.|[Einlagerung von Artikeln](warehouse-put-away-items.md)|
|Lagern Sie Artikel zwischen Lagerplätzen in dem Lager um.|[Umlagern von Artikeln](warehouse-move-items.md)|
|Kommissionieren Sie Artikel, die geliefert, umgelagert oder bei der Montage bzw. Produktion verbraucht werden, gemäß dem konfigurierten Lageraktivitätsvorgang.|[Kommissionieren von Artikeln](warehouse-pick-items.md)|
|Erfassen Sie die Lieferung von Artikeln aus Lagerorten, entweder mit nur einem Verkaufsauftrag, in einfachen Lagerorteinrichtungen oder mit einem Warenausgang, im Falle von halb- oder vollautomatisierter Lagerverarbeitung am Lagerort.|[Versenden von Artikeln](warehouse-how-ship-items.md)|  

## <a name="see-also"></a>Siehe auch  
[Lagerbesttand](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]