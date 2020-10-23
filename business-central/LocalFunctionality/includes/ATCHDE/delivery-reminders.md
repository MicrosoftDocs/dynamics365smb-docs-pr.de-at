---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1e7cb126ea06d96bd130d644948d08fd7e2e1a11
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959610"
---
Lieferbenachrichtigungen dienen dazu, überfällige Kreditorlieferungen zu verfolgen und Kreditoren an überfällige Lieferungen zu erinnern. Zur Erstellung von Lieferbenachrichtigungen müssen Sie Folgendes einrichten:

- Lieferbenachrichtigungsmethoden  

    Lieferbenachrichtigungsmethoden werden durch einen Code identifiziert, der Kreditoren zugewiesen werden muss. Um mehrere Einstellungskombinationen verwenden zu können, müssen Sie jeweils für jede Einstellung getrennt einen Code festlegen. Sie können eine beliebige Anzahl an Lieferbenachrichtigungsmethoden einrichten.  

- Lieferbenachrichtigungsstufen  

    Für jede Lieferbenachrichtigungsmethode müssen gesonderte Lieferbenachrichtigungstexte festgelegt werden. Diese Stufen bestimmen, wie oft Lieferbenachrichtigungen für eine bestimmte Methode erzeugt werden können. Stufe 1 ist die erste Lieferbenachrichtigung, die Sie für eine überfällige Lieferung erstellen. Stufe 2 ist die zweite Lieferbenachrichtigung und so weiter. Bei der Erstellung von Lieferbenachrichtigungen wird die Anzahl der zuvor erstellten Benachrichtigungen berücksichtigt und die für die aktuelle Anzahl definierte Methode verwendet.  

- Lieferbenachrichtigungstexte  

    Sie müssen für jede Lieferbenachrichtigungsstufe gesonderte Lieferbenachrichtigungstexte festlegen. Es gibt zwei Arten von Lieferbenachrichtigungstexten: Vortexte und Nachtexte. Der Vortext wird unter dem Kopf vor der Liste von Einträgen, die angemahnt werden, gedruckt. Der Nachtext wird nach dieser Liste gedruckt.  

Nach dem Einrichten der Lieferbestimmungen, -stufen und -texte müssen Sie den Kreditoren die entsprechenden Lieferanmahnungscodes zuweisen.  

Lieferbenachrichtigungen können manuell oder automatisch erstellt werden. Sie können den Batchauftrag **Lieferanmahnung erstellen** zum automatischen Erstellen von Lieferanmahnungen nutzen, damit Sie die Bestellungen auswählen können, für die Lieferanmahnungen erstellt werden müssen.  

Sie können Dokumente auch in Bezug auf Bestell- oder Auftragspositionen verfolgen.  

[!INCLUDE[d365fin](../../../includes/d365fin_md.md)] stellt die folgenden Berichte bereit:  

- **Reg. Lieferbenachrichtigung** – Zum Anzeigen der Lieferbenachrichtigungen für Kreditoren.  
- **Lieferbenachrichtigung - Test** - Zum Überprüfen der Lieferbenachrichtigungen vor deren Ausgabe.  
