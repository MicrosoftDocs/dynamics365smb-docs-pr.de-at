---
title: Exemplarische Vorgehensweise für Serviceaufträge für Serviceartikel
description: 'Dieser Artikel führt Sie durch mehrere Kernprozesse, die Serviceaufträge und Artikel betreffen.'
author: andreipa
ms.author: andreipa
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 05/31/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# <a name="walkthrough-of-service-orders-for-service-items"></a>Exemplarische Vorgehensweise für Serviceaufträge für Serviceartikel

Diese exemplarische Vorgehensweise demonstriert mehrere Kernprozesse:

- Erstellen Sie einen Ad-hoc-Serviceauftrag und registrieren Sie die Reparatur des Artikels
- Bereitstellung eines Leihartikels für den Kunden zur Reparatur
- Buchen und fakturieren Sie den Serviceauftrag
    
## <a name="creating-a-service-order"></a>Erstellen eines Serviceauftrags

### <a name="scenario"></a>Szenario

Charles, der Servicemanager, erstellt einen Serviceauftrag für ein Reparaturszenario und überlässt der Kundschaft für die Reparaturzeit ein Leihgerät.

### <a name="steps"></a>Schritte

1. Erstellen Sie den Serviceauftrag manuell für den Artikel, der repariert werden muss.
   1. Wählen Sie das Symbol ![Glühbirne, die die Funktion „Wie möchten Sie weiter verfahren“ öffnet.](../../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") aus. Symbol, geben Sie **Serviceaufträge** ein
   2. Wählen Sie die Aktion **Neu** aus.
   3. Geben Sie **10000** als Debitorennr. ein. Feld
   4. Wählen **REPARATUR** für das Feld **Serviceauftragstyp**.
   5. Wählen Sie in den Zeilen **S-100** als **Artikelnummer** aus.
2. Optional
   1. Wählen Sie die Zeilenaktion **Fehlerbehebung**, um mögliche Lösungen zu prüfen.
   2. Wählen Sie die Zeilenaktion **Problem/Resol. Code-Verhältnisse**
   3. Wählen Sie *GERÄUSCH* als **Symptomcode**
   4. Wählen Sie *5-2 Lautes Geräusch beim Brühen* als **Fehlercode** und schließen Sie die Seite. Fehlercode und Lösungscodes werden zeilenweise aktualisiert.
3. Leihen Sie einen Ersatz, während der Artikel repariert wird
   1. Wählen Sie in den Zeilen **LEIHGERÄT1** als Leihnummer aus. Bestätigen Sie die Ausgabe des Leihgeräts, indem Sie **Ja** auswählen, um das Leihgerät zu überlassen. 
   2. Wählen Sie die Funktionsaktion **Std.-Servicecodes abrufen**, wählen Sie den mit der Servicegruppe verknüpften Standardcode und dann **OK** aus.
   
### <a name="results"></a>Ergebnisse

- Für den Artikel wird ein Serviceauftrag erstellt
- Im Servicedokumentprotokoll des Serviceauftrags werden die Aktivitäten des Kreditgebers angezeigt.
- Der Kreditgeber verfügt über einen Hauptbucheintrag, der die Kreditvergabe widerspiegelt.
   

## <a name="register-performed-work-mark-loaner-as-returned"></a>Durchgeführte Arbeit registrieren, Leihgerät als zurückgegeben kennzeichnen.

### <a name="scenario-1"></a>Szenario

Der Servicetechniker markiert das Leihgerät als zurückgegeben und registriert die durchgeführten Arbeiten.

### <a name="steps-1"></a>Schritte

1. Suchen Sie die Serviceaufgabe und registrieren Sie die Zeit 
   1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](../../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") Symbol. Geben Sie **Serviceaufgaben** ein und wählen Sie dann den zugehörigen Link.
   2. Suchen Sie den Serviceauftrag, für den Sie die Zeit eingeben möchten.
   3. Wählen Sie die Aktion **Artikel-Arbeitsblatt** aus.
   4. Geben Sie die folgenden Informationen ein

    |Typ|Anz.|Menge|
    |----|---|--------|  
    |Option|SER102|2|

   4. Wählen Sie *FERTIG* im Feld **Reparaturstatuscode** aus
    
2. Leihgerät als zurückgegeben markieren
   1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](../../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") Symbol. Geben Sie **Leihgeräte** ein und wählen Sie dann den zugehörigen Link.
   2. Suchen Sie das Leihgerät, um es als zurückgegeben zu kennzeichnen.
   3. Wählen Sie die Aktion **Empfang**. 
   4. Bestätigen Sie die Rückgabe des Leihgeräts, indem Sie **Ja** auswählen, um das Leihgerät zurückzugeben.
      
### <a name="results-1"></a>Ergebnisse

- Im **Servicebelegprotokoll** des Serviceauftrags werden die Aktivitäten des Kreditgebers angezeigt.
- Der Kreditgeber verfügt über einen Sachposten, der den Empfang widerspiegelt.


### <a name="scenario-2"></a>Szenario

Charles, der Servicemanager, veröffentlicht den fertigen Serviceauftrag.

1. Suchen Sie den Serviceauftrag 
   1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](../../media/ui-search/search_small.png "Tell Me-Funktion") Symbol. Geben Sie **Serviceaufträge** ein und wählen Sie dann den zugehörigen Link.
   2. Suchen Sie den Serviceauftrag, den Sie buchen möchten.

2. Buchen Sie die Rechnung auf dem Serviceauftrag
   1. Wählen Sie die Aktion **Buchen**, um den Serviceauftrag abzuschließen. Wählen Sie die Aktion **Versand und fakturieren**, und wählen Sie dann **OK**.
   2. Bestätigen Sie das Öffnen der gebuchten Rechnung, indem Sie **Ja** auswählen. 
### <a name="results-2"></a>Ergebnisse

- Die **Gebuchte Servicerechnung** wird erstellt.
- die **Serviceposten**, die mit dem Artikel und der Ressource verbunden sind, werden erstellt

## <a name="see-also"></a>Siehe auch
[Exemplarische Vorgehensweise für Serviceverträge für Serviceartikel](service-contract-flow.md)  
[Dienst](../../service-service.md)
