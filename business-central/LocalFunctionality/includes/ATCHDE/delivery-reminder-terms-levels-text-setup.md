---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5cfc99bcbdf9a5037e8c87686cd65badf4ce544c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771498"
---
Zur Erstellung von Lieferbenachrichtigungen müssen Sie Folgendes einrichten:  

- Lieferbenachrichtigungsmethoden  
- Lieferbenachrichtigungsstufen  
- Lieferbenachrichtigungstexte  

Jede Lieferbenachrichtigungsmethoden verfügt über mindestens zwei Lieferbenachrichtigungsstufe und für jede Lieferbenachrichtigungsstufe können Sie Text angeben, der in die Lieferbenachrichtigung aufgenommen wird.  

## <a name="to-set-up-delivery-reminder-terms"></a>So richten Sie Lieferbenachrichtigungsmethoden ein  

1. Wählen Sie die ![Glühbirne, die das Tell Me Feature](../../../media/ui-search/search_small.png "Tell me-Funktion") Symbol öffnet, geben Sie **Lieferanmahnungsbedingungen** ein und wählen Sie dann den entsprechenden Link.  
2. Wählen Sie die Aktion **Neu**.  
3. Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Der Code für die Lieferbenachrichtigungsmethode. Sie können bis zu 10 alphanumerische Zeichen eingeben.|  
    |**Beschreibung**|Der Beschreibung für die Lieferbenachrichtigungsmethode. Sie können bis zu 30 alphanumerische Zeichen eingeben.|  
    |**Max. Anzahl Lieferbenachrichtigungen**|Die maximale Anzahl von Lieferbenachrichtigungen, die für eine Bestellung erstellt werden kann.<br /><br /> **HINWEIS:** Diese Höchstgrenze gilt für alle Benachrichtigungsstufen dieser Benachrichtigungsmethode zusammen. Wenn Sie z. B. drei Stufen definiert haben und **Max. Anzahl Lieferbenachrichtigungen** auf 5 festlegen, wird die erste Mahnung auf Stufe 1, die Zweite auf Stufe 2, die Dritte auf Stufe 3 erstellt.|  

4. Wählen Sie die Schaltfläche **OK** aus.  

## <a name="to-add-delivery-reminder-levels-to-a-delivery-reminder-term"></a>So fügen Sie einer Lieferanmahnungsmethode Lieferanmahnungsstufen hinzu  

1. Wählen Sie auf der Seite **Lieferanmahnungsmethoden** die Lieferanmahnung aus, der Sie Stufen hinzufügen möchten, und wählen Sie dann die Aktion **Bearbeiten**.  
2. Wählen Sie die Aktion **Neu**.  
3. Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Die Nummer der Lieferbenachrichtigungsstufe. Dieses Feld wird automatisch ausgefüllt.|  
    |**Berechnung Fälligkeitsdatum**|Die Formel für die Fälligkeitsdatumsberechnung der Lieferbenachrichtigung. Sie können eine Kombination von Zahlen zwischen 0 und 9999 sowie Datumscodes (T für Tag, WT für Wochentag, W für Woche, M für Monat, Q für Quartal oder J für Jahr) eingeben. Die Datumscodes bezeichnen die Berechnung desFälligkeitsdatums der Lieferbenachrichtigung fest. Sie können bis zu 20 Zeichen für die Berechnungsformel für den Fälligkeitstermin eingeben.|  

4. Wählen Sie die Schaltfläche **OK** aus.  

Für jede Lieferbenachrichtigungsstufe können Sie Textnachrichtigen definieren, die der Lieferbenachrichtigung hinzugefügt werden. Sie können Vortext definieren, der vor der Beschreibung der überfälligen Bestellung eingefügt wird, und Nachtext, der nach der Beschreibung der überfälligen Bestellung eingefügt wird.  

Im folgenden Verfahren wird beschrieben, wie Sie den Vortext einrichten. Diese Schritte gelten jedoch auch für das Einrichten von Nachtexten.  

## <a name="to-set-up-delivery-reminder-text-messages"></a>Einrichten von Lieferbenachrichtigungstexten  

1. Wählen Sie auf der Seite **Lieferanmahnungsstufen** eine Stufe aus, und wählen Sie dann die Aktion **Vortext**.  
2. Wählen Sie die Aktion **Neu**.  
3. Geben Sie im Feld **Beschreibung** den Vortext für die Lieferbenachrichtigung ein.  
4. Wählen Sie die Schaltfläche **OK** aus.  
