---
title: Artikel und Inventar synchronisieren
description: Synchronisierungen von Artikeln zwischen Shopify und Business Central einrichten und ausführen
ms.date: 05/27/2022
ms.topic: article
ms.service: dynamics365-business-central
author: AndreiPanko
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: c7aea0d0b3d9a8902e704a2d390d6a244e8cbbef
ms.sourcegitcommit: b353f06e0c91aa6e725d59600f90329774847ece
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 08/19/2022
ms.locfileid: "9317317"
---
# <a name="synchronize-items-and-inventory"></a>Artikel und Inventar synchronisieren

Die **Artikel** in [!INCLUDE[prod_short](../includes/prod_short.md)] sind gleichbedeutend mit *Produkte* in Shopify, einschließlich physischer Waren, digitaler Downloads, Dienstleistungen und Geschenkkarten, die Sie verkaufen. Es gibt zwei Hauptgründe für die Synchronisierung der Artikel:

1. Die Datenverwaltung wird hauptsächlich in [!INCLUDE[prod_short](../includes/prod_short.md)] durchgeführt. Sie müssen alle oder einige Daten nach Shopify exportieren und sie sichtbar machen. Sie können Artikelname, Beschreibung, Bild, Preise, Verfügbarkeit, Varianten, Lieferantendetails und Barcode exportieren. Nach dem Import können die Artikel sofort sichtbar werden oder sie können zuerst von einer verantwortlichen Person überprüft und erweitert werden.
2. Bei einer Bestellung von Shopify importiert wird, sind die Informationen zu den Artikeln für die Weiterverarbeitung des Dokuments in [!INCLUDE[prod_short](../includes/prod_short.md)] unerlässlich.

Diese beiden Szenarien sind immer aktiviert.

Ein drittes Szenario ist die Verwaltung von Daten in Shopify, importieren Sie diese Artikel jedoch in großen Mengen in [!INCLUDE[prod_short](../includes/prod_short.md)]. Dieses Szenario kann für Datenmigrationsereignisse hilfreich sein, wenn einen bestehenden Onlineshop mit einer neuen [!INCLUDE[prod_short](../includes/prod_short.md)]-Umgebung verbinden möchten.

## <a name="to-define-item-synchronizations"></a>So definieren Sie Artikelsynchronisierungen

1. Wählen Sie das Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") aus , und geben Sie **Shopify-Shop** ein. Öffnen Sie einen Shop, für den Sie die Artikelsynchronisierung konfigurieren möchten.
2. Wählen Sie im Feld **Artikel synchronisieren** die erforderliche Option aus. <br>In der folgenden Tabelle wird der Unterschied zwischen den Optionen beschrieben.

|Option|Description|
|------|-----------|
|**"Leer"**| Der Import von Produkten erfolgt zusammen mit dem Import von Bestellungen. Produkte werden nach Shopify exportiert, wenn Benutzer die Aktion **Artikel hinzufügen** über die Seite **Shopify-Produkte** ausführt. Dieser Prozess ist das Standardverhalten. |
|**Zu Shopify**| Wählen Sie diese Option, wenn Sie nach der ersten Synchronisierung, die durch die Aktion **Artikel hinzufügen** ausgelöst wurde, Produkte manuell mit der Aktion **Produkte synchronisieren** oder über eine Aufgabenwarteschlange für wiederkehrende Aktualisierungen aktualisieren möchten. Denken Sie daran, das Feld **Kann Shopify-Produkt aktualisiseren** zu aktivieren. Wenn es nicht aktiviert, entspricht es der Option **Leer**. Weitere Informationen finden Sie unter [Artikel nach Shopify exportieren](synchronize-items.md#export-items-to-shopify).|
|**Von Shopify**| Wählen Sie diese Option aus, wenn Sie planen, Produkte aus Shopify in großen Mengen zu importieren, indem Sie entweder manuell die Aktion **Produkt synchronisieren** oder die Auftragswarteschlange für wiederkehrende Aktualisierungen verwenden. Wenn keine Option ausgewählt ist, entspricht es der Option **Leer**. Weitere Einzelheiten zum Importieren von Artikeln finden Sie unter [Artikel aus Shopify importieren](synchronize-items.md#import-items-from-shopify).|

## <a name="import-items-from-shopify"></a>Artiekl aus Shopify importieren

Entweder importieren Sie Artikel aus Shopify in großen Mengen oder zusammen mit dem Import von Bestellungen. Diese Artikel werden zuerst den Tabellen **Shopify-Produkt** und **Shopify-Variante** hinzugefügt. Der Prozess kann mit den folgenden Einstellungen verwaltet werden:

|Feld|Description|
|------|-----------|
|**Unbekannte Artikel automatisch erstellen**|Wenn Shopify-Produkte und -Varianten in [!INCLUDE[prod_short](../includes/prod_short.md)] importiert werden, versucht die [!INCLUDE[prod_short](../includes/prod_short.md)]-Funktion immer, zuerst einen übereinstimmenden Datensatz in der Artikelliste zu finden. **SKU-Zuordnung** wirkt sich darauf aus, wie der Abgleich durchgeführt wird, und erstellt neue Artikel und/oder Artikelvarianten. Aktivieren Sie diese Option, wenn Sie einen neuen Artikel erstellen möchten oder kein übereinstimmender Datensatz vorhanden ist. Der neue Artikel wird mit importierten Daten und **Artikelvorlagencode** erstellt. Wenn diese Option nicht aktiviert ist, müssen Sie einen Artikel manuell erstellen und die Aktion **Kartenprodukt** auf der Seite **Shopify-Produkte** verwenden.|
|**Artikelvorlagencode**|Wird zusammen mit **Unbekannte Artikel automatisch erstellen** verwendet. <br> Wählen Sie die Vorlage aus, die für automatisch erstellte Elemente verwendet werden soll.|
|**SKU-Zuordnung**|Legen Sie fest, wie Sie den **SKU**-Wert verwenden möchten, der während der Zuordnung und Erstellung von Artikeln/Varianten aus Shopify importiert wurde. Weitere Informationen finden Sie unter [So wirken sich SKU und Strichcode, die in Shopify-Produkten definiert sind, auf die Zuordnung und Erstellung von Artikeln und Varianten aus](synchronize-items.md#how-skus-and-barcodes-defined-in-shopify-product-affects-mapping-and-creation-of-items-and-variants-in-business-central).|
|**SKU-Feldtrennzeichen**|Wird zusammen mit **SKU-Zuordnung** verwendet, die auf die Option **Artikelnr. und Variantencode** festgelegt ist.<br> Definieren Sie ein Trennzeichen, das zum Aufteilen der SKU verwendet werden soll. <br>Wenn Sie beispielsweise in Shopify die Variante mit SKU „1000/001“ erstellen, geben Sie „/“ in das Feld **SKU-Feldtrennzeichen** ein, um die Artikelnummer in [!INCLUDE[prod_short](../includes/prod_short.md)] als „1000“ und den Artikelvariantencode als „001“ zu erhalten.
|**Variantenpräfix**|Wird zusammen mit **SKU-Zuordnung** verwendet, die auf die Option **Variantencode** oder **Artikelnr. und Variantencode** als Fallback-Strategie festgelegt ist, wenn die SKU aus Shopify leer ist.<br>Wenn Sie die Artikelvariante automatisch in [!INCLUDE[prod_short](../includes/prod_short.md)] erstellen möchten, müssen Sie einen Wert in **Code** eingeben. Standardmäßig wird der im SKU-Feld definierte Wert aus Shopify verwendet. Wenn die SKU jedoch leer ist, wird Code generiert, der mit dem definierten Variantenpräfix und „001“ beginnt.|
|**Shopify Kann Artikel aktualisieren**| Wählen Sie diese Option aus, wenn Sie Artikel und/oder Varianten automatisch aktualisieren möchten.|

### <a name="how-skus-and-barcodes-defined-in-shopify-product-affects-mapping-and-creation-of-items-and-variants-in-business-central"></a>So wirken sich in SKU und Barcode definierte Shopify-Produkte auf die Zuordnung und Erstellung von Artikeln und Varianten in Business Central aus

Wenn Produkte von Shopify in die Tabellen **Shopify-Produkte** und **Shopify-Varianten** importiert werden, versucht [!INCLUDE[prod_short](../includes/prod_short.md)] vorhandene Datensätze zu finden. In der folgenden Tabelle wird der Unterschied zwischen den Optionen im Feld **SKU-Zuordnung** beschrieben.

|Option|Auswirkung auf die Zuordnung|Auswirkung auf die Erstellung|
|------|-----------------|------------------|
|**"Leer"**|Das SKU-Feld wird in der Artikelzuordnungsroutine nicht verwendet.|Keine Auswirkung auf die Erstellung des Elements. <br>Verhindert die Erstellung von Varianten. Ist im Verkaufsauftrag hilfreich, nur der Hauptartikel verwendet wird. Eine Variante kann weiterhin manuell über das Fenster **Shopify-Produkt** zugeordnet werden.|
|**Artikelnr.**|Legen Sie fest, ob das SKU-Feld die Artikelnummer enthält.|Keine Auswirkung auf die Erstellung des Elements ohne Varianten. Bei einem Artikel mit Varianten wird jede Variante als separater Artikel erstellt.<br> Wenn Shopify beispielsweise ein Produkt mit zwei Varianten aufweist und deren Lagerhaltungsdaten lauten „1000“ und „2000“, erstellt das System in [!INCLUDE[prod_short](../includes/prod_short.md)] zwei Artikel mit den Nummern „1000“ und „2000“.|
|**Variantencode**|Das SKU-Feld wird in der Artikelzuordnungsroutine nicht verwendet.|Keine Auswirkung auf die Erstellung des Elements. Beim Erstellen einer Artikelvariante dient der Wert des SKU-Felds als Code. Wenn die SKU leer ist, wird ein Code über das Feld **Variantenpräfix** erstellt.|
|**Artikelnr. und Variantencode**| Legen Sie fest, ob das SKU-Feld eine Artikelnummer enthält und der Artikelvariantencode durch den im Feld **SKU-Feldtrennzeichen** definierten Wert getrennt ist.|Beim Erstellen eines Artikels wird der erste Teil des Werts des SKU-Felds als **Nr.** verwendet. Wenn die SKU leer ist, wird eine Artikelnummer mit der Nummernserie generiert, die in **Artikelvorlagencode** oder **Artikelnummern** aus dem Fenster **Lagereinrichtung** definiert ist.<br>Beim Erstellen eines Artikels verwendet die Variantenfunktion den zweiten Teil des Werts des SKU-Felds als **Code**. Wenn die SKU leer ist, wird ein Code über das Feld **Variantenpräfix** erstellt.|
|**Kreditorenartikelnr.**| Legen Sie fest, ob das SKU-Feld die Kreditorenartikelnummer enthält. In diesem Fall wird die **Kred.-Artikelnr.** nicht im Fenster **Artikelkarte**, sondern die **Kred.-Artikelnr.** aus dem **Artikel/Lieferanten Katalog** verwendet. Wenn der gefundene Datensatz *Artikel/Lieferanten Katalog* einen Variantencode enthält, wird dieser Variantencode zum Zuordnen der Shopify-Variante verwendet.|Wenn ein entsprechender Kreditor in [!INCLUDE[prod_short](../includes/prod_short.md)] vorhanden ist, wird der SKU-Wert als **Kred.-Artikelnr.** in der **Artikelkarte** und als **Artikelreferenz** vom Typ „Kreditor“ verwendet. <br>Verhindert die Erstellung von Varianten. Dies ist nützlich, wenn Sie den Hauptartikel nur im Verkaufsauftrag verwenden möchten. Sie können weiterhin eine Variante manuell über das Fenster **Shopify-Produkt** zuordnen.|
|**Strichcode**| Legen Sie fest, ob das SKU-Feld einen Strichcode enthält. Es wird eine Suche unter **Artikelreferenzen** vom Typ „Kreditor“ durchgeführt. Wenn der gefundene Artikelreferenzdatensatz einen Variantencode enthält, wird dieser Variantencode zum Zuordnen der Shopify-Variante verwendet.|Keine Auswirkung auf die Erstellung des Elements. <br>Verhindert die Erstellung von Varianten. Dies kann nur dann hilfreich sein, wenn nur der Hauptartikel im Verkaufsauftrag verwendet wird. Eine Variante kann weiterhin manuell über das Fenster **Shopify-Produkt** zugeordnet werden.|

In der folgenden Tabelle wird die Auswirkung des Felds **Strichcode** beschrieben.

|Auswirkung auf die Zuordnung|Auswirkung auf die Erstellung|
|-----------------|------------------|
|Es wird eine Suche unter **Artikelreferenzen** vom Typ „Strichcode“ für den Wert durchgeführt, der im Feld „Strichcode“ in Shopify definiert ist. Wenn der Artikelreferenzdatensatz einen Variantencode enthält, wird dieser Variantencode zum Zuordnen der Shopify-Variante verwendet.|Der Barcode wird als **Artikelreferenz** für den Artikel und die Artikelvariante gespeichert.|

> [!NOTE]  
> Sie können die Zuordnung für die ausgewählten Produkte/Varianten oder alle importierten nicht zugeordneten Produkte auslösen, indem Sie wählen **Zuordnung von Produkten suchen** (für ausgewählte) oder **Zuordnung suchen** (für alle) auswählen.

## <a name="export-items-to-shopify"></a>Artikel nach Shopify exportieren

Wählen Sie die Elemente aus Ihrer Artikelliste aus, die nach Shopify exportiert werden. Verwenden Sie die Aktion **Artikel hinzufügen** aus dem Fenster **Shopify-Produkte**, um der Shopify-Produktliste Artikel hinzuzufügen.

Der Prozess des Artikelexports kann mit den folgenden Einstellungen verwaltet werden:

|Feld|Description|
|------|-----------|
|**Debitorenpreisgruppe**|Bestimmen Sie den Preis für einen Artikel in Shopify. Der Verkaufspreis dieser Debitorenpreisgruppe wird verwendet. Wenn keine Gruppe eingegeben wird, wird der Preis der Artikelkarte verwendet.|
|**Debitorenrabattgruppe**|Bestimmen Sie den Rabatt, der zur Berechnung des Preises eines Artikels in Shopify verwendet werden soll. Ermäßigte Preise sind im Feld **Preis** hinterlegt und der volle Preis wird im Feld **Vergleichen mit Preis** gespeichert.|
|**Erweiterten Text für Artikel synchronisieren**|Wählen Sie diese Option aus, um den erweiterten Text des Artikels zu synchronisieren. Da es der *Beschreibung* hinzugefügt wird, kann es HTML-Code enthalten. |
|**Artikelattribute synchronisieren**|Wählen Sie diese Option aus, um die Artikelattribute zu synchronisieren. Attribute werden als Tabelle formatiert und sind im Feld *Beschreibung* in Shopify enthalten.|
|**Sprachcode**|Wenn diese Option ausgewählt ist, werden die übersetzten Versionen für Titel, Attribute und erweiterten Text verwendet.|
|**SKU-Zuordnung**|Legen Sie fest, wie das SKU-Feld in Shopify ausgefüllt werden soll. Die folgenden Optionen werden unterstützt:<br> - **Artikelnr.** zur Verwendung der Artikelnr. für Produkte und Varianten.<br> - **Artikelnr. und Variantencode** zum Erstellen einer SKU, indem die Werte der beiden Felder verkettet werden. Für Artikel ohne Varianten wird nur die Artikelnummer verwendet.<br>- **Artikellieferantennr.** zur Verwendung der Artikellieferantennummer, die auf der *Artikelkarte* für Produkte und Varianten definiert ist.<br> - **Barcode** – verwendet **Artikelreferenz** vom Typ „Strichcode“. Diese Option berücksichtigt Varianten. |
|**SKU-Feldtrennzeichen**|Definieren Sie ein Trennzeichen für die Opton **Artikelnr. und Variantencode**.|
|**Verfolgter Lagerbestand**|Legen Sie fest, wie das Feld **Lagerbestand verfolgen** für Produkte ausgefüllt werden soll, die nach Shopify exportiert werden. Sie können Verfügbarkeitsinformationen von [!INCLUDE[prod_short](../includes/prod_short.md)] für Produkte in Shopify mit aktivierter Lagerbestandsverfolgung aktualisieren. Weitere Informationen finden Sie unter [Lagerbestand](synchronize-items.md#sync-inventory-to-shopify).|
|**Standardrichtlinie für Lagerbestand**|Wählen Sie *Verweigern* aus, um einen negativen Lagerbestand der Shopify-Seite zu vermeiden. |
|**Kann Shopify-Produkte aktualisieren**|Definieren Sie, ob [!INCLUDE[prod_short](../includes/prod_short.md)] Artikel nur erstellen oder auch aktualisieren kann. Wählen Sie diese Option aus, wenn Sie nach der ersten Synchronisierung, die durch die Aktion **Artikel hinzufügen** ausgelöst wurde, Produkte manuell mit der Aktion **Produkte synchronisieren** oder über eine Aufgabenwarteschlange für wiederkehrende Aktualisierungen aktualisieren möchten. Denken Sie daran, **Mit Shopify** im Feld **Artikelsynchronisierung** auszuwählen.|
|**Debitorenvorlagencode**|Wählen Sie die Standardvorlage, die während der Preisberechnung verwendet werden soll. Weitere Informationen finden Sie unter [Steuern einrichten](setup-taxes.md).|


### <a name="fields-mapping-overview"></a>Übersicht über Feldzuordnungen

|Shopify|Quelle beim Export aus [!INCLUDE[prod_short](../includes/prod_short.md)]|Ziel beim Importier in [!INCLUDE[prod_short](../includes/prod_short.md)]|
|------|-----------------|-----------------|
|Status|Entsprechend des **Status für erstellte Produkte** auf der **Shopify-Shop-Karte**. Weitere Informationen finden Sie unter [Ad-Hoc-Aktualisierungen von Shopify-Produkten](synchronize-items.md#ad-hock-updates-of-shopify-products).|Wird nicht verwendet.|
|Titel|**Beschreibung**. Wenn der Sprachcode definiert und eine entsprechende Artikelübersetzung vorhanden ist, wird anstelle der Beschreibung die Artikelübersetzung verwendet.|**Beschreibung**|
|Description|Kombiniert erweiterte Texte und Attribute, wenn entsprechende Schalter auf der Shopify-Shop-Karte aktiviert sind. Berücksichtigt Sprachcode.|Wird nicht verwendet.|
|SEO-Seitentitel|Fester Wert: leer, siehe [Ad-Hoc-Aktualisierungen von Shopify-Produkten](synchronize-items.md#ad-hock-updates-of-shopify-products). |Wird nicht verwendet.|
|SEO-Metabeschreibung|Fester Wert: leer, siehe [Ad-Hoc-Aktualisierungen von Shopify-Produkten](synchronize-items.md#ad-hock-updates-of-shopify-products). |Wird nicht verwendet.|
|Medien|**Bild**, weitere Informationen, siehe [Artikelbilder synchronisieren](synchronize-items.md#sync-item-images)|**Bild**|
|Preis|Die Berechnung des Endkundenpreises enthält die Artikelpreisgruppe, die Artikelrabattgruppe, den Währungscode und den Debitorenvorlagencode. |**VK-Preis**|
|Preisvergleich|Die Berechnung des Preises ohne Rabatt enthält die Artikelpreisgruppe, die Artikelrabattgruppe, den Währungscode und den Debitorenvorlagencode. |Wird nicht verwendet.|
|Kosten pro Artikel|**Einstandspreis**|**Einstandspreis**|
|SKU|Weitere Informationen finden Sie unter **SKU-Zuordnung** unter [Artikel nach Shopify exportieren](synchronize-items.md#export-items-to-shopify).| Weitere Informationen finden Sie unter [So wirken sich SKU und Strichcode, die in Shopify definiert sind, auf die Zuordnung und Erstellung von Artikeln und Varianten aus](synchronize-items.md#how-skus-and-barcodes-defined-in-shopify-product-affects-mapping-and-creation-of-items-and-variants-in-business-central).|
|Strichcode|**Artikelreferenzen** vom Typ „Strickcode“|**Artikelreferenzen** vom Typ „Strickcode“|
|Menge verfolgen|Entsprechend der Option **Verfolgter Lagerbestand** auf der **Shopify-Shop-Karte**. Weitere Informationen finden Sie unter [Lagerbestand](synchronize-items.md#sync-inventory-to-shopify).|Wird nicht verwendet.|
|Weiterverkaufen, wenn ein Artikel nicht mehr auf Lager ist|Entsprechend der Option **Standardrichtlinie für Lagerbestand** auf der **Shopify-Shop-Karte**. Nicht importiert.|Wird nicht verwendet.|
|Typ|**Beschreibung** von **Artikelkategoriencode**. Wenn der Typ nicht in Shopify angegeben ist, wird er als benutzerdefinierter Typ hinzugefügt.|**Artikelkategoriencode**. Zuordnung nach Beschreibung.|
|Kreditor|**Name** des Kreditors aus **Kreditorennr.** |**Kreditorennr.**-Zuordnung nach Name.|
|Gewichtung|**Bruttogewicht**.|Wird nicht verwendet.|
|Steuerpflichtig|Fester Wert: Aktiviert.|Wird nicht verwendet.|
|Steuercodes|**Steuergruppencode**. Nur für die Umsatzsteuer relevant. Weitere Informationen finden Sie unter [Steuern einrichten](setup-taxes.md). |Wird nicht verwendet.|

### <a name="tags"></a>Tags

Überprüfen Sie die importierten Tags in der Infobox **Tags** auf der Seite **Shopify-Produkt**. Wählen Sie zum Bearbeiten von Tags die Aktion **Tags** auf der Seite **Shopify-Produkt** aus.
Wenn die Option **Mit Shopify** im Feld **Artikel synchronisieren** ausgewählt ist, werden zugewiesene Tags bei der nächsten Synchronisierung nach Shopify exportiert.

## <a name="run-item-synchronization"></a>Artikelsynchronisierung ausführen

Die vollständige oder teilweise Synchronisierung von Artikeln kann auf viele verschiedene Arten durchgeführt werden.

### <a name="initial-sync-of-items-from-business-central-to-shopify"></a>Anfängliche Synchronisierung von Artikeln aus Business Central mit Shopify

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") , rufen Sie **Shopify-Produkte** auf, und wählen Sie den zugehörigen Link aus.
2. Wählen Sie die Aktion **Artikel hinzufügen** aus.
3. Geben Sie im Feld **Shop-Code** den ersten Code ein. Wenn Sie das Fenster **Shopify-Produkt** über das Fenster **Shop-Karte** aufrufen, wird der Shop-Code automatisch ausgefüllt.
4. Definieren Sie nach Bedarf Filter für Artikel. Sie können beispielsweise nach Artikelnummer oder nach Artikelkategoriencode filtern.
5. Wählen Sie **OK** aus.

Die resultierenden Artikel werden automatisch in Shopify mit Preisen erstellt, Bilder und Lagerbestände sind jedoch nicht enthalten. Der Vorgang kann einige Zeit dauern, wenn eine große Anzahl von Artikeln hinzugefügt wird.

### <a name="sync-products-from-shopify-to-business-central"></a>Produkte aus Shopify mit Business Central synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") , geben Sie **Shopify-Shop** ein, und wählen Sie den entsprechenden Link aus.
2. Wählen Sie den Shop aus, für den Sie Artikel synchronisieren möchten, um die Seite **Shopify-Shop-Karte** zu öffnen.
3. Wählen Sie die Aktion **Produkte synchronisieren** aus.

Verwenden Sie alternativ die Aktion **Produkte synchronisieren** im Fenster **Shopify-Produkte** aus, oder suchen Sie nach dem Stapelverarbeitungsauftrag **Produkte synchronisieren**.

Sie können die durchzuführende Aufgabe so planen, dass sie automatisiert ausgeführt werden. Weitere Informationen finden Sie unter [Wiederkehrende Aufgaben planen](background.md#to-schedule-recurring-tasks).

### <a name="ad-hock-updates-of-shopify-products"></a>Ad-Hoc-Aktualisierungen von Shopify-Produkten

Beim Aktualisieren der Datensätze in der Tabelle **Shopify-Produkt** werden die folgenden Änderungen mit Shopify synchronisiert.

Aktualisieren:

* **Status** – Sie können zwischen „Aktiv“, „Archiviert“ oder „Entwurf“ auswählen.
* **SEO-Titel**
* **SEO-Beschreibung**

Löschung:

Basierend auf dem Wert in **Aktion für entfernte Produkte** auf der **Shopify-Shop-Karte**, wird das Produkt in Shopify aktualisiert, wenn der Datensatz von der Seite **Shopify-Produkte** gelöscht wird.

* **Leer** – Es wird keine Aktion ausfgeführt. Der Benutzer muss die erforderliche Aktion ggf. über die Shopify-Verwaltung ausführen.
* **Status auf Entwurf** – Der Status des Produkts in Shopify ist auf *Entwurf* festgelegt.
* **Status auf Archiviert** – Das Produkt ist in Shopify archiviert.

## <a name="sync-item-images"></a>Artikelbilder synchronisieren

Die Synchronisierung von Bildern kann für synchronisierte Artikel konfiguriert werden. Die folgenden Optionen stehen zur Auswahl:

* **Leer** – Bildsynchronisation ist deaktiviert.
* **Zu Shopify** – Bilder von Artikeln werden nach Shopify exportiert
* **Von Shopify** – Bilder von Shopify werden nach [!INCLUDE[prod_short](../includes/prod_short.md)] importiert

Die Bildsynchronisation kann auf zwei Arten initialisiert werden.

### <a name="sync-product-images-from-the-shopify-shop-window"></a>Produktbilder über das Fenster „Shopify-Shop“ synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion") , geben Sie **Shopify-Shops** ein, und wählen Sie den entsprechenden Link aus.
2. Wählen Sie den Shop aus, für den Sie Bilder synchronisieren möchten, um die Seite **Shopify-Shop-Karte** zu öffnen.
3. Wählen Sie die Aktion **Produktbilder synchronisieren** aus.

### <a name="sync-product-images-from-the-shopify-products-window"></a>Produktbilder über das Fenster „Shopify-Produkte“ synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion") , rufen Sie **Shopify-Produkte** auf, und wählen Sie den zugehörigen Link aus.
2. Wählen Sie die Aktion **Produktbilder synchronisieren** aus.

### <a name="image-synchronization-remarks"></a>Anmerkungen zur Bildsynchronisation

* Beim Exportieren von Bildern von [!INCLUDE[prod_short](../includes/prod_short.md)] nach Shopify werden die neuen Bilder Shopify hinzugefügt und alte Bilder bleiben intakt. Wenn ein Bild in [!INCLUDE[prod_short](../includes/prod_short.md)] aktualisiert wird, müssen Sie alte Bilder über die Shopify-Verwaltung löschen.
* Bilder, die nach Shopify exportiert werden und den von Shopify definierten Anforderungen nicht entsprechen, werden nicht importiert. Weitere Informationen finden Sie unter [Produktmedientypen auf help.shopify.com](https://help.shopify.com/en/manual/products/product-media/product-media-types#images).

## <a name="sync-prices-with-shopify"></a>Preise mit Shopify synchronisieren

Preise können für synchronisierte Artikel auf die unten beschriebene Weise exportiert werden.

### <a name="sync-prices-from-the-shopify-products-window"></a>Preise über das Fenster „Shopify-Produkte“ synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion"). , rufen Sie **Shopify-Produkte** auf, und wählen Sie den zugehörigen Link aus.
2. Wählen Sie die Aktion **Preise mit Shopify synchronisieren** aus.

### <a name="price-calculation-remarks"></a>Anmerkungen zur Preisberechnung

* Für die Preisberechnung ist es wichtig, dass sich ein Wert im Feld **Standarddebitorenvorlage** befindet. Weitere Informationen finden Sie unter [Steuern einrichten](setup-taxes.md).
* Geben Sie einen **Währungscode** ein, wenn Ihr Onlineshop eine andere Währung als MW verwendet. Für die angegebene Währung müssen Wechselkurse konfiguriert sein. Wenn Ihr Onlineshop dieselbe Währung verwendet wie [!INCLUDE[prod_short](../includes/prod_short.md)], lassen Sie das Feld leer.
* Bei der Bestimmung eines Preises verwendet [!INCLUDE[prod_short](../includes/prod_short.md)] die Logik „Niedrigster Preis“. Das heißt, wenn der auf der Artikelkarte definierte Stückpreis niedriger ist als der in der Preisgruppe definierte, wird der Einzelpreis aus der Artikelkarte verwendet.

## <a name="sync-inventory-to-shopify"></a>Lagerbestand mit Shopify synchronisieren

Die Synchronisierung des Lagerbestands kann für bereits synchronisierte Artikel konfiguriert werden. Dazu müssen zwei Bedingungen erfüllt sein:

1. Die Nachverfolgung von Lagerbeständen muss für ein Produkt in Shopify aktiviert werden. Erwägen Sie beim Exportieren von Artikeln nach Shopify die Aktivierung von **Verfolgter Lagerbestand** auf der **Shopify-Shop**-Karte. Weitere Informationen finden Sie unter [Artikel nach Shopify exportieren](synchronize-items.md#export-items-to-shopify).
2. Die Synchronisierung des Lagerbestands muss für **Shopify-Standorte** aktiviert sein.

### <a name="to-enable-inventory-sync"></a>So aktivieren Sie die Synchronisierung des Lagerbestands

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion") , geben Sie **Shopify-Shop** ein, und wählen Sie den entsprechenden Link aus.
2. Wählen Sie den Shop aus, für den Sie den Lagerbestand synchronisieren möchten, um die Seite **Shopify-Shop-Karte** zu öffnen.
3. Wählen Sie die Aktion **Standorte** aus, um **Shopify-Shop-Standorte** zu öffnen.
4. Wählen Sie die Aktion **Shopify-Standorte abrufen** aus, um in Shopify definierten Standorte zu importieren. Sie befinden sich in den Einstellungen für [**Standorte**](https://www.shopify.com/admin/settings/locations) in Ihrer **Shopify-Verwaltung**.
5. Fügen Sie im Feld **Standortfilter** Standorte hinzu, wenn Sie nur den Lagerbestand bestimmter Standorte einbeziehen möchten. Sie können beispielsweise *OST|WEST* eingeben, sodass nur Lagerbestände dieser beiden Standorte für den Verkauf über den Onlineshop verfügbar sind.
6. Heben Sie die Auswahl des Umschalters **Deaktiviert** auf, um die Synchronisierung des Lagerbestands für ausgewählte Shopify-Standorte zu deaktivieren.

Die Synchronisierung des Lagerbestands auf zwei Arten initialisieren.

### <a name="sync-inventory-from-the-shopify-shop-window"></a>Lagerbestand über das Fenster „Shopify-Shop“ synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion") , geben Sie **Shopify-Shops** ein, und wählen Sie den entsprechenden Link aus.
2. Wählen Sie den Shop aus, für den Sie den Lagerbestand synchronisieren möchten, um die Seite **Shopify-Shop-Karte** zu öffnen.
3. Wählen Sie die Aktion **Lagerbestand synchronisieren** aus.

### <a name="sync-inventory-from-the-shopify-products-window"></a>Lagerbestand über das Fenster „Shopify-Produkte“ synchronisieren

1. Wechseln Sie zum Suchsymbol ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet](../media/ui-search/search_small.png "Tell Me-Funktion") , rufen Sie **Shopify-Produkte** auf, und wählen Sie den zugehörigen Link aus.
2. Wählen Sie die Aktion **Lagerbestand synchronisieren** aus.

### <a name="inventory-remarks"></a>Anmerkungen zum Lagerbestand

* Der Konnektor berechnet den **Verfügbarkeitssaldo** und exportiert ihn nach Shopify.
* Sie können die von Shopify empfangenen Bestandsinformationen auf der Seite **Infobox „Shopify-Bestand“** überprüfen. In dieser Infobox erhalten Sie einen Überblick über den Shopify-Bestand und den zuletzt berechneten Bestand in [!INCLUDE[prod_short](../includes/prod_short.md)]. Pro Standort ist ein Datensatz verfügbar.
* Wenn die Bestandsinformationen in Shopify sich vom **Verfügbarkeitssaldo** in [!INCLUDE[prod_short](../includes/prod_short.md)] unterscheiden, wird der Bestand in Shopify aktualisiert.

## <a name="see-also"></a>Siehe auch

[Erste Schritte mit dem Konnektor für Shopify](get-started.md)  