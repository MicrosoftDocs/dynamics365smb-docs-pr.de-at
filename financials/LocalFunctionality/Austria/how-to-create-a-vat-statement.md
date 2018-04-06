---
title: So erstellen Sie eine MwSt.-Abrechnung
description: "Sie können einen regelmäßigen Bericht der MsSt.-Transaktionen übermitteln. Die MwSt.-Abrechnung wird als FDF-Datei übermittelt. Dieses Dateiformat entspricht einer bearbeitbaren PDF-Datei der Steuerbehörde."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 8d60e9fb9565aa94a1440cba4ac34ab3bf213601
ms.contentlocale: de-at
ms.lasthandoff: 03/22/2018

---
<span data-ttu-id="8ba2a-104"><<<<<<< KOPF:financials/LocalFunctionality/Austria/how-to-create-a-vat-statement.md</span><span class="sxs-lookup"><span data-stu-id="8ba2a-104"><<<<<<< HEAD:financials/LocalFunctionality/Austria/how-to-create-a-vat-statement.md</span></span>
# <a name="create-a-vat-statement"></a><span data-ttu-id="8ba2a-105">Erstellen einer MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8ba2a-105">Create a VAT Statement</span></span>
=======
# <a name="create-a-vat-statement"></a><span data-ttu-id="8ba2a-106">Erstellen einer MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8ba2a-106">Create a VAT Statement</span></span>
>>>>>>> <span data-ttu-id="8ba2a-107">refs/remotes/origin/Update13:archive/LocalFunctionality/Austria/how-to-create-a-vat-statement.md [!INCLUDE[d365fin](../../includes/d365fin_md.md)] ermöglicht das Einreichen eines periodischen Berichts von MwSt.-Abrechnungen.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-107">refs/remotes/origin/Update13:archive/LocalFunctionality/Austria/how-to-create-a-vat-statement.md [!INCLUDE[d365fin](../../includes/d365fin_md.md)] allows you to submit a periodic report of VAT transactions.</span></span> <span data-ttu-id="8ba2a-108">Die MwSt.-Abrechnung wird als FDF-Datei übermittelt. Dieses Dateiformat entspricht einer bearbeitbaren PDF-Datei der Steuerbehörde.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-108">The VAT statement is submitted as a FDF file that corresponds with an editable PDF file from the tax authorities.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="8ba2a-109">Vor der Erstellung der MwSt.-Erklärung müssen Sie detaillierte Informationen zu Ihrer Firmenadresse im Fenster „Firmendaten” angeben.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-109">You must fill in detailed information about your company address in the Company Information window before you create the VAT statement.</span></span> <span data-ttu-id="8ba2a-110">Zu diesen Angaben zählen Straße, Hausnummer, Etage und Zimmernummer.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-110">This includes information about street, building, floor, and room number.</span></span> <span data-ttu-id="8ba2a-111">Diese Informationen werden in die FDF-Datei aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-111">This information is included in the FDF file.</span></span>  

## <a name="to-create-a-vat-statement"></a><span data-ttu-id="8ba2a-112">So erstellen Sie eine MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8ba2a-112">To create a VAT statement</span></span>  

1.  <span data-ttu-id="8ba2a-113">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), geben Sie **MwSt.-Abrechnung AT** ein, und wählen Sie dann den zugehörigen Link.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Statement AT**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8ba2a-114">Füllen Sie im Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-114">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="8ba2a-115">Feld</span><span class="sxs-lookup"><span data-stu-id="8ba2a-115">Field</span></span>|<span data-ttu-id="8ba2a-116">Description</span><span class="sxs-lookup"><span data-stu-id="8ba2a-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="8ba2a-117">**Startdatum**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-117">**Starting Date**</span></span>|<span data-ttu-id="8ba2a-118">Gibt das Startdatum der MwSt.-Periode an.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-118">Specifies the start date of the VAT period.</span></span>|  
    |<span data-ttu-id="8ba2a-119">**Enddatum**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-119">**Ending Date**</span></span>|<span data-ttu-id="8ba2a-120">Gibt das Enddatum der MwSt.-Periode an.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-120">Specifies the end date of the VAT period.</span></span>|  
    |<span data-ttu-id="8ba2a-121">**MwSt.-Posten einschließen**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-121">**Include VAT Entries**</span></span>|<span data-ttu-id="8ba2a-122">Gibt an, ob offene oder geschlossene oder sowohl offene als auch geschlossene MwSt.-Posten einbezogen werden.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-122">Specifies if you want to include VAT entries that are either open or closed, or both open and closed entries.</span></span>|  
    |<span data-ttu-id="8ba2a-123">**MwSt.-Posten einschließen**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-123">**Include VAT Entries**</span></span>|<span data-ttu-id="8ba2a-124">Gibt an, ob nur MwSt.-Posten aus der angegebenen Periode oder auch MwSt.-Posten aus der vorhergehenden Periode eingebogen werden.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-124">Specifies if you want to include VAT entries that are from the specified period or also include entries from before the period.</span></span>|  
    |<span data-ttu-id="8ba2a-125">**Berichtstyp**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-125">**Reporting Type**</span></span>|<span data-ttu-id="8ba2a-126">Markieren Sie, ob diese MwSt.-Abrechnung den vierteljährlichen Bericht, den monatlichen Bericht oder einen Bericht zu einer anderen Periode darstellt.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-126">Select if this VAT statement is the quarterly report, monthly report, or if it applies to another period.</span></span>|  
    |<span data-ttu-id="8ba2a-127">**Positionen prüfen**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-127">**Check Positions**</span></span>|<span data-ttu-id="8ba2a-128">Wählen Sie diese Option, um die Positionen der MwSt.-Abrechnung während des Exports zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-128">Select to verify the positions of the VAT statement during the export.</span></span>|  
    |<span data-ttu-id="8ba2a-129">**Auf ganze Zahlen runden**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-129">**Round to Whole Numbers**</span></span>|<span data-ttu-id="8ba2a-130">Hier wird ausgewählt, dass Beträge auf ganze Zahlen gerundet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-130">Select to round amounts to whole numbers.</span></span>|  
    |<span data-ttu-id="8ba2a-131">**Für Zahlung von Verbindlichkeiten genutzter Überschuss**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-131">**Surplus Used to Pay Dues**</span></span>|<span data-ttu-id="8ba2a-132">Wählen Sie diese Option, wenn ein möglicher Überschuss zur Deckung anderer Verbindlichkeiten verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-132">Select to use a potential surplus to cover other charges.</span></span>|  
    |<span data-ttu-id="8ba2a-133">**Weitere per Post geschickte Rechnungen**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-133">**Additional Invoices sent via Mail**</span></span>|<span data-ttu-id="8ba2a-134">Wählen Sie diese Option, wenn Sie zusätzliche Informationen senden werden.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-134">Select if you will send additional information.</span></span>|  
    |<span data-ttu-id="8ba2a-135">**Nummer §6 Abs. 1**</span><span class="sxs-lookup"><span data-stu-id="8ba2a-135">**Number §6 Abs. 1**</span></span>|<span data-ttu-id="8ba2a-136">Geben Sie die Nummer gemäß §6 Absatz 1 an, wenn steuerfreie Einnahmen ohne Vorsteuerabzug geltend machen möchten.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-136">Specify the number according to §6 section 1 if you want to claim tax-free revenues without input tax reduction.</span></span>|  

3.  <span data-ttu-id="8ba2a-137">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-137">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="8ba2a-138">Speichern oder öffnen Sie nach der entsprechenden Aufforderung die generierte XML-Datei und FDF-Datei.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-138">When prompted, choose to save or open the generated XML file and FDF file.</span></span>  

<span data-ttu-id="8ba2a-139">Wenn Ihre MwSt-Abrechnung fehlerfrei ist, können Sie die FDF-Datei an die Steuerbehörde übermitteln.</span><span class="sxs-lookup"><span data-stu-id="8ba2a-139">If your VAT statement does not contain errors, you can now submit the FDF file to the tax authorities.</span></span> <span data-ttu-id="8ba2a-140">Weitere Informationen finden Sie online unter [Finanz-Online portal](http://go.microsoft.com/fwlink/?LinkId=239929).</span><span class="sxs-lookup"><span data-stu-id="8ba2a-140">For more information, see the [Finanz-Online portal](http://go.microsoft.com/fwlink/?LinkId=239929).</span></span>  

## <a name="see-also"></a><span data-ttu-id="8ba2a-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8ba2a-141">See Also</span></span>  
[<span data-ttu-id="8ba2a-142">MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8ba2a-142">VAT Reporting</span></span>](vat-reporting.md)

