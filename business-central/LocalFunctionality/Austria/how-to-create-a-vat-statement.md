---
title: So erstellen Sie eine MwSt.-Abrechnung
description: "Sie können einen regelmäßigen Bericht der MsSt.-Transaktionen übermitteln. Die MwSt.-Abrechnung wird als FDF-Datei übermittelt, die einer bearbeitbaren PDF-Datei von der Steuerbehörde entspricht."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8c0535db9e0745f23290c733f1c992e9d61d463f
ms.contentlocale: de-at
ms.lasthandoff: 03/22/2018

---
# <a name="create-a-vat-statement"></a><span data-ttu-id="7cdec-104">Erstellen einer MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="7cdec-104">Create a VAT Statement</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="7cdec-105"> ermöglicht Ihnen, einen regelmäßigen Bericht der MsSt.-Transaktionen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="7cdec-105"> allows you to submit a periodic report of VAT transactions.</span></span> <span data-ttu-id="7cdec-106">Die MwSt.-Abrechnung wird als FDF-Datei übermittelt. Dieses Dateiformat entspricht einer bearbeitbaren PDF-Datei der Steuerbehörde.</span><span class="sxs-lookup"><span data-stu-id="7cdec-106">The VAT statement is submitted as a FDF file that corresponds with an editable PDF file from the tax authorities.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="7cdec-107">Vor der Erstellung der MwSt.-Erklärung müssen Sie detaillierte Informationen zu Ihrer Firmenadresse im Fenster „Firmendaten” angeben.</span><span class="sxs-lookup"><span data-stu-id="7cdec-107">You must fill in detailed information about your company address in the Company Information window before you create the VAT statement.</span></span> <span data-ttu-id="7cdec-108">Zu diesen Angaben zählen Straße, Hausnummer, Etage und Zimmernummer.</span><span class="sxs-lookup"><span data-stu-id="7cdec-108">This includes information about street, building, floor, and room number.</span></span> <span data-ttu-id="7cdec-109">Diese Informationen werden in die FDF-Datei aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="7cdec-109">This information is included in the FDF file.</span></span>  

## <a name="to-create-a-vat-statement"></a><span data-ttu-id="7cdec-110">So erstellen Sie eine MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="7cdec-110">To create a VAT statement</span></span>  

1.  <span data-ttu-id="7cdec-111">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), geben Sie **MwSt.-Abrechnung AT** ein, und wählen Sie dann den zugehörigen Link.</span><span class="sxs-lookup"><span data-stu-id="7cdec-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Statement AT**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7cdec-112">Füllen Sie im Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="7cdec-112">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="7cdec-113">Feld</span><span class="sxs-lookup"><span data-stu-id="7cdec-113">Field</span></span>|<span data-ttu-id="7cdec-114">Description</span><span class="sxs-lookup"><span data-stu-id="7cdec-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="7cdec-115">**Startdatum**</span><span class="sxs-lookup"><span data-stu-id="7cdec-115">**Starting Date**</span></span>|<span data-ttu-id="7cdec-116">Gibt das Startdatum der MwSt.-Periode an.</span><span class="sxs-lookup"><span data-stu-id="7cdec-116">Specifies the start date of the VAT period.</span></span>|  
    |<span data-ttu-id="7cdec-117">**Enddatum**</span><span class="sxs-lookup"><span data-stu-id="7cdec-117">**Ending Date**</span></span>|<span data-ttu-id="7cdec-118">Gibt das Enddatum der MwSt.-Periode an.</span><span class="sxs-lookup"><span data-stu-id="7cdec-118">Specifies the end date of the VAT period.</span></span>|  
    |<span data-ttu-id="7cdec-119">**MwSt.-Posten einschließen**</span><span class="sxs-lookup"><span data-stu-id="7cdec-119">**Include VAT Entries**</span></span>|<span data-ttu-id="7cdec-120">Gibt an, ob offene oder geschlossene oder sowohl offene als auch geschlossene MwSt.-Posten einbezogen werden.</span><span class="sxs-lookup"><span data-stu-id="7cdec-120">Specifies if you want to include VAT entries that are either open or closed, or both open and closed entries.</span></span>|  
    |<span data-ttu-id="7cdec-121">**MwSt.-Posten einschließen**</span><span class="sxs-lookup"><span data-stu-id="7cdec-121">**Include VAT Entries**</span></span>|<span data-ttu-id="7cdec-122">Gibt an, ob nur MwSt.-Posten aus der angegebenen Periode oder auch MwSt.-Posten aus der vorhergehenden Periode eingebogen werden.</span><span class="sxs-lookup"><span data-stu-id="7cdec-122">Specifies if you want to include VAT entries that are from the specified period or also include entries from before the period.</span></span>|  
    |<span data-ttu-id="7cdec-123">**Berichtstyp**</span><span class="sxs-lookup"><span data-stu-id="7cdec-123">**Reporting Type**</span></span>|<span data-ttu-id="7cdec-124">Markieren Sie, ob diese MwSt.-Abrechnung den vierteljährlichen Bericht, den monatlichen Bericht oder einen Bericht zu einer anderen Periode darstellt.</span><span class="sxs-lookup"><span data-stu-id="7cdec-124">Select if this VAT statement is the quarterly report, monthly report, or if it applies to another period.</span></span>|  
    |<span data-ttu-id="7cdec-125">**Positionen prüfen**</span><span class="sxs-lookup"><span data-stu-id="7cdec-125">**Check Positions**</span></span>|<span data-ttu-id="7cdec-126">Wählen Sie diese Option, um die Positionen der MwSt.-Abrechnung während des Exports zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7cdec-126">Select to verify the positions of the VAT statement during the export.</span></span>|  
    |<span data-ttu-id="7cdec-127">**Auf ganze Zahlen runden**</span><span class="sxs-lookup"><span data-stu-id="7cdec-127">**Round to Whole Numbers**</span></span>|<span data-ttu-id="7cdec-128">Hier wird ausgewählt, dass Beträge auf ganze Zahlen gerundet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7cdec-128">Select to round amounts to whole numbers.</span></span>|  
    |<span data-ttu-id="7cdec-129">**Für Zahlung von Verbindlichkeiten genutzter Überschuss**</span><span class="sxs-lookup"><span data-stu-id="7cdec-129">**Surplus Used to Pay Dues**</span></span>|<span data-ttu-id="7cdec-130">Wählen Sie diese Option, wenn ein möglicher Überschuss zur Deckung anderer Verbindlichkeiten verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7cdec-130">Select to use a potential surplus to cover other charges.</span></span>|  
    |<span data-ttu-id="7cdec-131">**Weitere per Post geschickte Rechnungen**</span><span class="sxs-lookup"><span data-stu-id="7cdec-131">**Additional Invoices sent via Mail**</span></span>|<span data-ttu-id="7cdec-132">Wählen Sie diese Option, wenn Sie zusätzliche Informationen senden werden.</span><span class="sxs-lookup"><span data-stu-id="7cdec-132">Select if you will send additional information.</span></span>|  
    |<span data-ttu-id="7cdec-133">**Nummer §6 Abs. 1**</span><span class="sxs-lookup"><span data-stu-id="7cdec-133">**Number §6 Abs. 1**</span></span>|<span data-ttu-id="7cdec-134">Geben Sie die Nummer gemäß §6 Absatz 1 an, wenn steuerfreie Einnahmen ohne Vorsteuerabzug geltend machen möchten.</span><span class="sxs-lookup"><span data-stu-id="7cdec-134">Specify the number according to §6 section 1 if you want to claim tax-free revenues without input tax reduction.</span></span>|  

3.  <span data-ttu-id="7cdec-135">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="7cdec-135">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="7cdec-136">Speichern oder öffnen Sie nach der entsprechenden Aufforderung die generierte XML-Datei und FDF-Datei.</span><span class="sxs-lookup"><span data-stu-id="7cdec-136">When prompted, choose to save or open the generated XML file and FDF file.</span></span>  

<span data-ttu-id="7cdec-137">Wenn Ihre MwSt-Abrechnung fehlerfrei ist, können Sie die FDF-Datei an die Steuerbehörde übermitteln.</span><span class="sxs-lookup"><span data-stu-id="7cdec-137">If your VAT statement does not contain errors, you can now submit the FDF file to the tax authorities.</span></span> <span data-ttu-id="7cdec-138">Weitere Informationen finden Sie online unter [Finanz-Online portal](http://go.microsoft.com/fwlink/?LinkId=239929).</span><span class="sxs-lookup"><span data-stu-id="7cdec-138">For more information, see the [Finanz-Online portal](http://go.microsoft.com/fwlink/?LinkId=239929).</span></span>  

## <a name="see-also"></a><span data-ttu-id="7cdec-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7cdec-139">See Also</span></span>  
[<span data-ttu-id="7cdec-140">MwSt.-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="7cdec-140">VAT Reporting</span></span>](vat-reporting.md)

