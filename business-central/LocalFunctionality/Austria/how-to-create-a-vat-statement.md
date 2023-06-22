---
title: So erstellen Sie eine MwSt.-Abrechnung
description: 'Sie können einen regelmäßigen Bericht der MsSt.-Transaktionen übermitteln. Die MwSt.-Abrechnung wird als FDF-Datei übermittelt, die einer bearbeitbaren PDF-Datei von der Steuerbehörde entspricht.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="create-a-vat-statement" />Erstellen einer MwSt.-Abrechnung
[!INCLUDE[prod_short](../../includes/prod_short.md)] ermöglicht Ihnen, einen regelmäßigen Bericht der MsSt.-Transaktionen zu übermitteln. Die MwSt.-Abrechnung wird als FDF-Datei übermittelt, die einer bearbeitbaren PDF-Datei von der Steuerbehörde entspricht.  

> [!NOTE]  
>  Mit Gültigkeit ab dem 1. Juli 2020 haben die österreichischen Behörden als vorübergehende Maßnahme zur Förderung der Wirtschaft in Bereichen, die hart von COVID-19 getroffen wurden, die Mehrwertsteuer für bestimmte Gastronomiedienstleistungen auf 5 % gesenkt. Wenn Sie Debitoren oder Kreditoren in den betroffenen Bereichen haben, müssen Sie MwSt-Buchungsgruppen erstellen, die den korrekten MwSt-Satz widerspiegeln, und diese für Transaktionen verwenden, die ab dem 1. Juli 2020 erstellt wurden. Um sicherzustellen, dass die neuen 5%-MwSt.-Transaktionen korrekt in die MwSt.-Abrechnungen aufgenommen werden, führen Sie die Aktion **MwSt.-Abrechnung aktualisieren** im Feld **Suche** aus. Dadurch wird die MwSt.-Erklärung neu erstellt und die 5%-Transaktionen eingezogen, die im entsprechenden Feld in der offiziellen PDF-Vorlage für die MwSt.-Erklärung zur Berichterstattung bereit sind. Stellen Sie außerdem sicher, dass Sie die offizielle PDF-Vorlage für die MwSt-Berichterstattung erhalten.  

> [!IMPORTANT]  
>  Vor der Erstellung der MwSt.-Erklärung müssen Sie detaillierte Informationen zu Ihrer Firmenadresse auf der Seite „Firmendaten” angeben. Zu diesen Angaben zählen Straße, Hausnummer, Etage und Zimmernummer. Diese Informationen werden in die FDF-Datei aufgenommen.  

## <a name="to-create-a-vat-statement" />So erstellen Sie eine MwSt.-Abrechnung

1.  Wählen Sie das Symbol ![Glühbirne, die die Funktion „Wie möchten Sie weiter verfahren“ öffnet.](../../media/ui-search/search_small.png "Tell me-Funktion") aus. Geben Sie **MwSt.-Abrechnung AT** ein, und wählen Sie dann den zugehörigen Link aus.  
2.  Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Datumsart für Zeitraum**|Gibt den Datumstyp der Periode an, ab der MwSt.-Posten in der Stapelverarbeitung erfasst werden.|
    |**Startdatum**|Gibt das Startdatum der MwSt.-Periode an.|  
    |**Enddatum**|Gibt das Enddatum der MwSt.-Periode an.|  
    |**MwSt.-Posten einschließen**|Gibt an, ob offene oder geschlossene oder sowohl offene als auch geschlossene MwSt.-Posten einbezogen werden.|  
    |**MwSt.-Posten einschließen**|Gibt an, ob nur MwSt.-Posten aus der angegebenen Periode oder auch MwSt.-Posten aus der vorhergehenden Periode eingebogen werden.|  
    |**Berichtstyp**|Markieren Sie, ob diese MwSt.-Abrechnung den vierteljährlichen Bericht, den monatlichen Bericht oder einen Bericht zu einer anderen Periode darstellt.|  
    |**Positionen prüfen**|Wählen Sie diese Option, um die Positionen der MwSt.-Abrechnung während des Exports zu überprüfen.|  
    |**Auf ganze Zahlen runden**|Hier wird ausgewählt, dass Beträge auf ganze Zahlen gerundet werden sollen.|  
    |**Für Zahlung von Verbindlichkeiten genutzter Überschuss**|Wählen Sie diese Option, wenn ein möglicher Überschuss zur Deckung anderer Verbindlichkeiten verwendet werden soll.|  
    |**Weitere per Post geschickte Rechnungen**|Wählen Sie diese Option, wenn Sie zusätzliche Informationen senden werden.|  
    |**Nummer §6 Abs. 1**|Geben Sie die Nummer gemäß §6 Absatz 1 an, wenn steuerfreie Einnahmen ohne Vorsteuerabzug geltend machen möchten.|  

3.  Wählen Sie die Schaltfläche **OK** aus.  
4.  Speichern oder öffnen Sie nach der entsprechenden Aufforderung die generierte XML-Datei und FDF-Datei.  

Wenn Ihre MwSt-Abrechnung fehlerfrei ist, können Sie die FDF-Datei an die Steuerbehörde übermitteln. Weitere Informationen finden Sie online unter [Finanz-Online portal](https://go.microsoft.com/fwlink/?LinkId=239929).  

## <a name="see-also" />Siehe auch
[MwSt.-Abrechnung](vat-reporting.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
