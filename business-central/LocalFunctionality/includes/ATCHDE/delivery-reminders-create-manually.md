---
author: brentholtorf
ms.topic: include
ms.date: 11/21/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---

In [!INCLUDE[prod_short](../../../includes/prod_short.md)] können Sie Lieferbenachrichtigungen erstellen, wenn eine Bestellung nicht wie erwartet geliefert wurde. Sie können eine einzelne Lieferbenachrichtigung manuell erstellen oder Sie können Lieferbenachrichtigungen für alle überfälligen Lieferungen erstellen.  

> [!NOTE]
> Um Lieferanmahnungen zu erstellen, müssen Sie die Lieferanmahnungsbestimmungen, -stufen und -texte eingerichtet haben.

## So erstellen Sie Lieferantenbenachrichtigungen manuell  

1. Wählen Sie ![Das Glühbirnen-Symbol, das die Funktion „Wie möchten Sie weiter verfahren“ öffnet.](../../../media/ui-search/search_small.png "Tell me-Funktion") aus. Geben Sie **Lieferanmahnung** ein, und wählen Sie dann den zugehörigen Link aus.  
2. Wählen Sie die Aktion **Neu** aus.  
3. Füllen Sie auf der Seite **Lieferanmahnung** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Die eindeutige Kennnummer für die Lieferbenachrichtigung.|  
    |**Kreditorennr**|Gibt die Nummer des Kreditors an, für den Sie eine Lieferbenachrichtigung buchen möchten.<br /><br /> Wenn Sie die Kreditorennummer auswählen, werden **Name**, **Adresse**, **PLZ Code/Ort** und **Kontakt** Felder automatisch ausgefüllt.|  
    |**Buchungsdatum**|Gibt das Buchungsdatum der Lieferbenachrichtigung an. Dieses Datum wird in alle Lieferbenachrichtigung kopiert.|  
    |**Belegdatum**|Gibt das Dokumentdatum der Lieferbenachrichtigung an. Dieses Datum wird auch verwendet, um das Fälligkeitsdatum der Lieferbenachrichtigung zu bestimmen. Sie können das Buchungsdatum bei Bedarf ändern.|  
    |**Mahnstufe**|Lieferbenachrichtigungsstufe. Dieser Wert basiert auf der Anzahl von gesendeten Lieferbenachrichtigungen.|  
    |**Mahnmethodencode**|Gibt den Lieferbenachrichtigungscode für den Kreditor an.|  
    |**Fälligkeitsdatum**|Gibt das Fälligkeitsdatum der Lieferbenachrichtigung an.|  

4. Wählen Sie die Aktion **Mahnungszeile vorschlagen**.  

    Wenn es überfällige Lieferungen vom angegebenen Kreditor gibt, werden diese der Lieferbenachrichtigung hinzugefügt.  

5. Wählen Sie die Schaltfläche **OK** aus.  

    Lieferbenachrichtigung wurde erstellt. So können die Lieferbenachrichtigungen ausgeben und erstellen.  
