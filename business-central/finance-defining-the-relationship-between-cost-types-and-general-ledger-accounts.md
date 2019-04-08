---
title: Definieren der Beziehung zwischen Kostenarten und Sachkonten | Microsoft Docs
description: Lernen, wie die beiden Felder definiert werden, die die Beziehung zwischen Kostenart und Sachkonto festlegen
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: f80e9b6276d26adffb5e3208ffefbf98d7f7ff96
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/08/2019
ms.locfileid: "823471"
---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a>Definieren der Beziehung zwischen Kostenarten und Sachkonten
Das Verbindung zwischen der Kostenart und dem Sachkonto wird in der Kostenart und im Sachkonto erstellt.  

* Das Feld **Fibu-Kontenbereich** in der Tabelle **Kostenart** bestimmt, welche Sachkonten zu einer Kostenart gehören.  
* Das **Kostenartennummer** Feld im Kontenplan bestimmt, zu welcher Kostenart ein Sachkonto gehört.  

Diese beiden Felder werden automatisch ausgefüllt, wenn Sie die **Kostenarten aus Kontenplan abrufen**-Funktion verwenden.  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a>Beziehung zwischen Sachkonten und Kostenarten  
Zwischen Sachkonten und Kostenarten besteht eine n:1-Beziehung. Mehrere Sachkonten können zu einer Kostenart gehören, aber jedes Sachkonto gehört nur zu einer Kostenart. In der folgenden Tabelle werden die Details der Beziehung beschrieben.  

|Verbindungen|**Sachkontobereich**|**Kostenartnr.**|  
|------------------|------------------------------------------------|-------------------------------------------|  
|Ein Sachkonto für jede Kostenart|Ein Sachkonto|Eine Kostenart|  
|Mehrere Sachkonten für eine Kostenart|Sachkontobereich, z. B. 7110 ... 7193 für jedes Sachkonto|Für jedes Sachkonto im Bereich gibt es nur eine Kostenart|  
|Kostenarten ohne entsprechende Sachkonten|<Empty>||  
|Sachkonten, deren Posten nicht übertragen werden||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a>Kostenarten ohne Beziehung zum Sachkonto  
Eine Kostenart hat möglicherweise keine Beziehung zu Sachkonten, wenn eine der folgenden Bedingungen zutrifft:  

* Konten für die betriebliche Buchhaltung, wie Berech. Zinsen und Abschreibungen, entnehmen nur Kosten aus der betrieblichen Buchhaltung.  
* Helfende Kostenarten, wie Kostenarten 9901, 9902 und 9903 in der [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datenbank, werden als Haben- und Sollbeträge für Zuordnungen verwendet.  
* Das helfende Konto, 9920 in der [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datenbank, enthält tatsächliche Zugänge, die die Differenz zwischen Kosten und Ausgaben des Sachkontos anzeigen.  

## <a name="see-also"></a>Siehe auch  
[Kostenrechnung](finance-manage-cost-accounting.md)  
[Einrichten der Kostenrechnung](finance-set-up-cost-accounting.md)   
[Informationen zur Kostenrechnung](finance-about-cost-accounting.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
