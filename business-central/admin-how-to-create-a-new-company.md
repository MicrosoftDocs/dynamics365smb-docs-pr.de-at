---
title: 'So geht es: Ein neues Unternehmen erstellen | Microsoft Docs'
description: Um RapidStart Services zu verwenden, werden Tabellen und Seiten erstellt, aber sie enthalten keine Daten.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7583837e515a4fd5fb415fe1b482512e7edf6b5a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754033"
---
# <a name="create-a-new-company"></a>Erstellen eines neuen Mandanten.
Um RapidStart Services für [!INCLUDE[prod_short](includes/prod_short.md)] zu verwenden, müssen Sie zunächst einen neuen Mandanten erstellen, für den Sie eine Debitoren-Implementierung durchführen wollen. Bei der Erstellung eines neuen Mandanten werden die [!INCLUDE[prod_short](includes/prod_short.md)]-Standardtabellen und -seiten erstellt, aber sie enthalten keine Daten.

Darüber hinaus können Sie bestimmte Einrichtungsdaten bei Ihrem Unternehmen anwenden, nachdem Sie es initialisiert haben. Die Informationen werden in einem Konfigurationspaket, eine .rapidstart-Datei bereitgestellt, die Inhalt in einem komprimierten Format bereitstellt.  

Beispielkonfigurationspakete, einschließlich landes-/regionspezifischer Dateien, sind im CRONUS-Demounternehmen enthalten. Verwenden Sie die folgende Vorgehensweisen, um das Beispielkonfigurationspaket mit einem neuen Mandanten zu verwenden.  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a>Beispielskonfigurationspaket BASICCONFIG verwenden  
1. Öffnen Sie das Unternehmen „CRONUS International Ltd.”. Weitere Informationen finden Sie unter [Ändern der Grundeinstellungen](ui-change-basic-settings.md).
2. Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell Me-Funktion") aus, geben Sie **Konfigurationspakete** ein, und wählen Sie dann den zugehörigen Link.  
3. Wählen Sie das BASICCONFIG-Paket von der Liste aus, und wählen **Exportpaket**.  

Verwenden Sie das folgende Vorgehen, um einen neuen Mandanten zu erstellen, und verwenden Sie das BASICCONFIG-Paket als Teil des Prozesses.  

## <a name="to-create-a-new-company"></a>So erstellen Sie einen neuen Mandanten:  
1. Erstellen eines neuen Mandanten. Weitere Informationen finden Sie unter [Neue Mandanten erstellen in[!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).
2. Vom RapidStart Services-Implementierungs-Rollencenter können Sie das Konfigurationspaket jetzt importieren, das Sie aus CRONUS International Ltd. exportierten.

Nachdem Sie ein neues Unternehmen erstellt haben, werden einige Tabellen automatisch ausgefüllt, auch wenn keine Unternehmensvorlage angewendet wird. Beispielsweise können Sie die Standardcodes für Buchungen und Stapeltransaktionen auf der Seite **Quellencode** prüfen. Wenn Sie eine lokale Version von [!INCLUDE[prod_short](includes/prod_short.md)] zur Verfügung stellen, sollten Sie diese Tabelle prüfen und auf sämtliche lokale sprachliche Aspekte achten.

## <a name="about-data-tables"></a>Info zu Datentabellen
[!INCLUDE[prod_short](includes/prod_short.md)]  Datentabellen liegen in zwei Haupttypen vor: Master und Einrichtung. Wenn Sie eine Mandantkonfiguration erstellen, können Sie diese Arten verwenden, um Ihre Konfigurationsstrategie zu konzentrieren.  

### <a name="master-data-tables"></a>Stammdatentabellen  
In der folgenden Tabelle sind einige Bespiele für -Stammdatentabellen aufgeführt. Wenn Sie einen neuen Mandanten initialisieren, sind diese Tabellen leer.  

|Tabellennr.|Tabellenname|  
|-------------------|--------------------|  
|15|Sachkonto|  
|18|Debitor|  
|23|Kreditor|  
|27|Option|  
|5050|Kontakt|  

### <a name="setup-data-tables"></a>Einrichtungsdatentabellen  
Die folgende Tabelle enthält Beispiele für Einrichtungsdatentabellen, in denen Sie Einrichtungsinformationen im Konfigurationsfragebogen erfassen. Diese Tabellen enthalten Basisinformationen, wenn der Mandant erstellt wird.  

|Tabellennr.|Tabellenname|  
|-------------------|--------------------|  
|98|Finanzbuchhaltung Einrichtung|  
|311|Debitoren & Verkauf Einr.|  
|312|Kreditoren & Einkauf Einr.|  
|313|Lagereinrichtung|  

Zusätzlich zu den Einrichtungsdatentabellen hat [!INCLUDE[prod_short](includes/prod_short.md)] auch Datentabellen, die Kernangaben zu dem Unternehmen und seinen Geschäftsprozesse enthalten. In der folgenden Tabelle werden einige dieser Felder aufgeführt:  

|Tabellennr.|Tabellenname|  
|-------------------|--------------------|  
|3|Zahlungsbedingungen|  
|4|Währung|  
|6|Debitorenpreisgruppen|  
|5700|Lagerhaltungsdaten|

  

## <a name="see-also"></a>Siehe auch  
[Konfigurationen für neue Mandanten übernehmen](admin-apply-configuration-to-new-companies.md)  
[Mandanten mit RapidStart Services einrichten](admin-set-up-a-company-with-rapidstart.md)  
[Verwaltung](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]