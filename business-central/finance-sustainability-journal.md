---
title: Nachhaltigkeitsposten erfassen
description: 'Erfahren Sie, wie Sie Treibhausgasemissionen (THG-Emissionen) erfassen.'
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, journal'
ms.search.form: '6216, 6219, 6220'
ms.date: 08/19/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Nachhaltigkeitsposten erfassen

Benutzer können Treibhausgasemissionen (THG) manuell im Nachhaltigkeitsbuch erfassen, indem sie Nachhaltigkeitsjournale oder beliebige Arten von einkaufsbezogenen Dokumenten verwenden.  

> [!NOTE]
> Die Verwendung jeglicher Art von kaufbezogenen Dokumenten zur Erfassung von Treibhausgasemissionen (THG) ist ab  *2024 Veröffentlichungszyklus 2 möglich*.  

## Nachhaltigkeits-Buch.-Blätter

Nachhaltigkeits-Buch.-Blätter sind für die Nachverfolgung und Erfassung von Nachhaltigkeitsaktivitäten konzipiert und bieten dazu dieselbe Benutzererfahrung wie andere Buch.-Blätter in Business Central. Benutzende, die über die erforderlichen Informationen verfügen, können Emissionen manuell in ein Buch.-Blatt eingeben. Falls diese Informationen nicht vorliegen, können sie alternativ integrierte Formeln verwenden, um die Emissionen auf der Grundlage spezifischer bekannter Parameter, die verschiedenen Arten von Quellen und Konten entsprechen, genau zu berechnen.

Die in ein Buch.-Blatt eingegebenen Informationen sind temporär und können geändert werden, solange sie sich in diesem Buch.-Blatt befinden. Wenn Sie das Buch.-Blatt buchen, werden die Informationen in Nachhaltigkeitsposten auf einzelnen Nachhaltigkeitskonten übertragen, wo sie nicht geändert werden können. Sie können jedoch Storno- oder Korrekturbuchungen vornehmen.

### Buch-Blattvorlagen und -namen verwenden

Es gibt standardmäßig zwei Nachhaltigkeits-Buch.-Blattvorlagen: die Standardvorlage und die wiederkehrende Vorlage.

Sie können zu jeder Buch.-Blattvorlage mehrere Buch.-Blattnamen als Buch-Stapel erstellen. Wählen Sie hierzu auf der Seite **Nachhaltigkeits-Buch.-Blattvorlagen** die Aktion **Batch** aus und erstellen Sie dann auf der neuen Seite den neuen **Nachhaltigkeits-Buch.-Blattbatch**. So können Sie beispielsweise für jeden Emissionsscope einen eigenen Buch.-Blattbatch festlegen, indem Sie die Option **Emissionsscope** verwenden und dann einen der drei vorhandenen Scopes wählen. Sie können für jeden Batch die Werte **Quellcode** und **Ursachencode** hinzufügen oder ändern.

> [!TIP]
> Wenn Sie über viele Zeilen verfügen, können Sie das Fehlerrisiko verringern, indem Sie für jede Emissionsart einen Buch.-Blattbatch anlegen. Alternativ können Sie für alle Emissionsarten auch den normalen Batch verwenden.

### Nachhaltigkeits-Buch.-Blätter überprüfen

Sie können auf der Seite **Nachhaltigkeitseinrichtung** eine Hintergrundprüfung einschalten, um Verzögerungen beim Buchen zu vermeiden. Wenn bei der Arbeit am Nachhaltigkeits-Buch.-Blatt Fehler auftreten, informiert die Prüfung Sie und verhindert, dass das Buch.-Blatt gebucht wird.

Wenn Sie die Prüfung aktivieren, werden in der Infobox **Buch.-Blatt-Prüfung** Probleme in der aktuellen Zeile und im gesamten Batch angezeigt. Die Überprüfung erfolgt, wenn Sie einen Buch.-Blattbatch laden und wenn Sie eine andere Buchungsblattzeile auswählen. Die Kachel **Probleme insgesamt** in der Infobox zeigt an, wie viele Probleme [!INCLUDE [prod_short](includes/prod_short.md)] insgesamt gefunden hat. Durch Anklicken der Kachel können Sie eine Übersicht der Probleme öffnen.

### Mit Nachhaltigkeits-Buch.-Blättern arbeiten

Um mit Nachhaltigkeitszeitschriften zu arbeiten, folgen die Schritte:

1. Wählen Sie die ![Glühbirne, welche die 3. „Sie wünschen ...“-Funktion öffnet.](media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") Symbol. Geben Sie **Nachhaltigkeits-Buch.-Blatt** ein und wählen Sie dann den zugehörigen Link.
2. Geben Sie auf der Seite **Nachhaltigkeits-Buch.-Blatt** so viele Zeilen ein, wie Sie mit demselben Batch buchen möchten.
3. Sie können das Feld **Belegart** leer lassen oder **Rechnung** oder **Gutschrift** auswählen.
4. Im Feld **Kontonr.** können Sie nur nicht gesperrte Nachhaltigkeitskonten auswählen, wenn das Feld **Direktbuchung** ausgewählt ist und das Feld **Buchungsart** auf **Buchung** festgelegt ist. Außerdem muss für die Konten eine Kategorie und eine Unterkategorie konfiguriert sein.

    > [!NOTE]
    > Wenn Sie einen Batch verwenden, bei dem der Emissionsscope konfiguriert ist, muss der Wert **Emissionsscope** im Nachhaltigkeitskonto mit dem Wert **Emissionsscope** in dem verwendeten Batch übereinstimmen.

5. Sie können die Beträge entweder manuell buchen oder Formeln verwenden.

    - Wenn Sie über genaue Informationen zu den Emissionen verfügen und diese buchen möchten (d. h., die Informationen stehen auf der erhaltenen Rechnung), müssen Sie das Feld **Manuelle Eingabe** auswählen, um anzugeben, dass Sie die Beträge manuell eingeben. In diesem Fall können Sie Ihre Daten nicht direkt in die Felder **Kraftstoff/Strom**, **Entfernung**, **Benutzerdefinierter Betrag**, **Installationsmultiplikator** und **Zeitfaktor** eingeben, da sie nicht bearbeitbar sind. Die Felder **CO2-Emission**, **CH4-Emission** und **N2O-Emission** bleiben jedoch bearbeitbar und Sie können Ihre Daten direkt in diese Felder eingeben.
    - Wenn Sie die Emission nicht genau kennen und berechnen müssen, aktivieren Sie das Feld **Manuelle Eingabe** nicht. In diesem Fall werden die Felder **CO2-Emission**, **CH4-Emission** und **N2O-Emission** unbearbeitbar. Sie können Ihre Berechnungsdetails jedoch basierend auf der von Ihnen verwendeten Formel eingeben. Weitere Informationen zu den Formeln, die in der **Kategorie des Nachhaltigkeitskontos** festgelegt sind, finden Sie unter [Nachhaltigkeitskontenplan und Nachhaltigkeitssachkonto](finance-sustainability-accounts-ledger.md#account-categories).

6. Um das Buch.-Blatt zu buchen, wählen Sie die Aktion **Buchen** aus. Wenn Sie in einem Nachhaltigkeits-Buch.-Blatt buchen, werden Posten im Nachhaltigkeitssachkonto generiert.

Falls Ihre Formel auf der Option **Aus Finanzbuchhaltung berechnen** in der Kategorie des Nachhaltigkeitskontos beruht, müssen Sie die Aktion **Betrag aus Sachposten erfassen** verwenden, bevor Sie das Buch.-Blatt buchen, um die Emissionen basierend auf dieser Datenquelle zu berechnen. Darüber hinaus müssen Sie, Wenn Sie nach dem Ausfüllen der Buchblattzeilen Änderungen an den Emissionsfaktoren vorgenommen haben, die Aktion **Neu berechnen** auswählen, um den richtigen Betrag im Buch.-Blatt zu erhalten.

### Wiederkehrende Buch.-Blätter

Ein wiederkehrendes Buch.-Blatt ist ein Nachhaltigkeits.-Buch-Blatt mit spezifischen Feldern zur Verwaltung von Transaktionen, die Sie häufig und allenfalls mit wenigen Änderungen buchen. Dabei handelt es sich beispielsweise um Nachhaltigkeitstransaktionen wie Strom, Wärme oder andere ähnliche Transaktionen. Sie können mithilfe wiederkehrender Buch.-Blätter feste und variable Beträge buchen.

Wenn Sie ein wiederkehrendes Buch.-Blatt verwenden, müssen Sie Posten, die Sie regelmäßig buchen, nur einmal erstellen. Informationen wie Konten, Dimensionen und Dimensionswerte bleiben nach der Buchung im Buch.-Blatt erhalten. Sie können jedes Mal, wenn Sie buchen, die notwendigen Änderungen vornehmen.

Das Feld **Wiederkehrende Methode** ist wichtig. Es bestimmt, wie der Betrag in der Buchungsblattzeile nach der Buchung gehandhabt wird. Wenn Sie beispielsweise bei jeder Buchung der Zeile den gleichen Betrag verwenden, können Sie das Feld **F Fest** auswählen, damit der Betrag nach dem Buchen unverändert bleibt. Wenn Sie dieselben Konten und denselben Text in der Zeile verwenden, der Betrag aber bei jeder Buchung variiert, wählen Sie die Option **V Variable** aus, um den Betrag nach dem Buchen zu löschen.

Auch das Feld **Wiederholungsrate** ist wichtig und muss festgelegt werden. Dabei handelt es sich um ein Datumsformelfeld, das bestimmt, wie oft der Eintrag in der Buchungsblattzeile gebucht werden soll. Mehr dazu erfahren Sie unter [Verwenden von Datumsformeln](ui-enter-date-ranges.md#use-date-formulas).

Das Feld **Ablaufdatum** bestimmt das Datum, an dem die Zeile das letzte Mal gebucht werden soll. Die Zeile wird nach diesem Datum nicht mehr gebucht. Die Verwendung des Feldes **Ablaufdatum** hat den Vorteil, dass die Zeile nicht sofort aus dem Buch.-Blatt gelöscht wird. Sie können ein späteres Datum eingeben, so dass Sie die Zeile auch in der Zukunft verwenden können. Wenn das Feld leer ist, wird die Zeile jedes Mal gebucht, bis sie aus dem Buch.-Blatt gelöscht wird.

## Kauf Belege  

Um die Aufzeichnung von Treibhausgasemissionen (THG) in allen einkaufsbezogenen Dokumenten zu ermöglichen, müssen Sie auf der Seite  **Nachhaltigkeits-Setup**  die Option  **Emissionen in Einkaufsdokumenten verwenden**  Auswählen.  

Um mit kaufbezogenen Dokumenten zu arbeiten, folgen Sie die Schritte:

1. Wählen Sie die ![Glühbirne, welche die 3. „Sie wünschen ...“-Funktion öffnet.](media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") Symbol und:  
   1. Geben Sie  **Einkaufsrechnungen**  ein, wenn Sie eine Rechnung als  **Dokumenttyp** wünschen, und Auswählen Sie dann die zugehörige verknüpfen.  
   2. Geben Sie  **Bestellungen**  ein, wenn Sie als  **Dokumententyp** bestellen möchten, und Auswählen Sie dann das zugehörige verknüpfen.  
2. Füllen Sie Kopfzeile und Zeilen anhand der folgenden Anleitung  [zum Arbeiten mit Einkaufsrechnungen und Bestellungen](purchasing-how-record-purchases.md) aus.
3. Wenn auf der Rechnung Ihres Lieferanten Informationen zu Emissionen vorhanden sind, wählen Sie in den Belegzeilen die entsprechende  **Nachhaltigkeitskontonummer**  aus und fügen Sie Emissionswerte mithilfe eines der folgenden Felder hinzu (je nachdem, was Sie verfolgen möchten und welche Emissionen auf Ihrer physischen Rechnung stehen):  **CO2-Emission**,  **CH4-Emission** oder  **N2O-Emission**.

    > [!NOTE]
    > Bei den von Ihnen in die Emissionsfelder eingetragenen Werten handelt es sich um Festbeträge pro Zeile, diese werden nicht mit dem Feld  **Menge**  multipliziert. Sie können die  **Nachhaltigkeitskontonummer** nur verwenden, wenn das Feld  **Typ**  (**Optionswerte**)  **Artikel**  oder  **Sachkonto** ist. Sie können keine  **Ressourcen** oder  **Gebühr (Artikel)** **Optionswerte** verwenden. 

4. Wenn Sie die Gesamtemissionen vor der Buchung sehen möchten, können Sie die Statistikseite öffnen und im Inforegister  **Nachhaltigkeit**  die gesamten gebuchten Emissionen sowie die Emissionen für die Buchung pro Dokument (alle kaufbezogenen Dokumente) finden.   
5. Buchen Sie die Belege und öffnen Sie eine neue  **gebuchte Einkaufsrechnung**.
6. Klicken Sie auf die Aktion Auswählen **Einträge suchen**, und Sie sehen, dass Sie auf der Seite  **Einträge suchen** den Eintrag  **Nachhaltigkeitsbucheintrag** als einen der zugehörigen Einträge haben.

> [!NOTE]
> Wenn Sie das Dokument buchen, erstellt das System für jede Einkaufszeile, für die Sie eine  **Nachhaltigkeitskontonummer**  haben, einen unabhängigen  **Nachhaltigkeitshauptbucheintrag** mit der  **Rechnung** als  **Dokumentart**  und derselben  **Dokumentnummer.**

> [!NOTE]
> Sie können auch eine  **Einkaufsgutschrift** erstellen und buchen. Sie können dies manuell tun oder eine der folgenden Optionen verwenden:  **Abbrechen**,  **Korrigieren** oder  **Korrekturgutschrift erstellen** . In diesem Fall kopiert das System die vorhandenen Werte aus der gebuchten Rechnung.  

## Siehe auch 

[Finanzen](finance.md)    
[Nachhaltigkeitsverwaltung – Übersicht](finance-manage-sustainability.md)    
[Nachhaltigkeits-Setup](finance-sustainability-setup.md)    
[Diagramm der Nachhaltigkeitskonten und -posten](finance-sustainability-accounts-ledger.md)    
[Ad-hoc-Analysen von Nachhaltigkeitsdaten](ad-hoc-analysis-sustainability.md)    
[Nachhaltigkeitsberichte und -analysen in Business Central](sustainability-reports.md)   
[Nachhaltigkeits-API](/dynamics365/business-central/dev-itpro/api-sustainability/sustainability-api?toc=/dynamics365/business-central/toc.json)    
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
