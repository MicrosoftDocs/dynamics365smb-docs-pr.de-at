---
title: 'Gewusst wie: Druck von Listenberichten für Kreditorenzahlungen'
description: Die Liste Kreditorenzahlungen zeigt eine Liste von Zahlungen für jeden Kreditor an. Der Bericht kann Zahlungen chronologisch oder nach Kreditor gruppiert sortieren.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 22ae6893392cbeed13ced701e219a3137f057bcf
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878735"
---
# <a name="print-vendor-payments-list-reports"></a><span data-ttu-id="cab58-104">Gewusst wie: Druck von Listenberichten für Kreditorenzahlungen</span><span class="sxs-lookup"><span data-stu-id="cab58-104">Print Vendor Payments List Reports</span></span>
<span data-ttu-id="cab58-105">Die Liste **Kreditorenzahlungen** zeigt eine Liste von Zahlungen für jeden Kreditor an.</span><span class="sxs-lookup"><span data-stu-id="cab58-105">The **Vendor Payments List** report provides a list of payments for each vendor.</span></span> <span data-ttu-id="cab58-106">Der Bericht kann Zahlungen chronologisch oder nach Kreditor gruppiert sortieren.</span><span class="sxs-lookup"><span data-stu-id="cab58-106">The report can sort payments chronologically or grouped by vendor.</span></span>  

## <a name="to-print-the-vendor-payments-list-report"></a><span data-ttu-id="cab58-107">Gewusst wie: Druck von Listenberichten für Kreditorenzahlungen</span><span class="sxs-lookup"><span data-stu-id="cab58-107">To print the vendor payments list report</span></span>  

1.  <span data-ttu-id="cab58-108">Wählen Sie das Symbol ![Suche nach Seite oder Bericht](../../media/ui-search/search_small.png "Suche nach Seiten- oder Berichtssymbolen"), geben Sie **Liste Kreditorenzahlungen** ein und wählen Sie dann den entsprechenden Link.</span><span class="sxs-lookup"><span data-stu-id="cab58-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Payments List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cab58-109">Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="cab58-109">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cab58-110">Feld</span><span class="sxs-lookup"><span data-stu-id="cab58-110">Field</span></span>|<span data-ttu-id="cab58-111">Description</span><span class="sxs-lookup"><span data-stu-id="cab58-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cab58-112">**Sortieren**</span><span class="sxs-lookup"><span data-stu-id="cab58-112">**Sorting**</span></span>|<span data-ttu-id="cab58-113">Gibt den sortierten Auftrag an.</span><span class="sxs-lookup"><span data-stu-id="cab58-113">Specifies the sort order.</span></span> <span data-ttu-id="cab58-114">Sie können chronologisch oder nach Kreditor sortieren.</span><span class="sxs-lookup"><span data-stu-id="cab58-114">You can sort by vendor or chronologically.</span></span> <span data-ttu-id="cab58-115">Wenn Sie nach Kreditor sortieren, finden Sie eine Zwischensumme für jeden Kreditor.</span><span class="sxs-lookup"><span data-stu-id="cab58-115">If you sort by vendor, you will see a subtotal for each vendor.</span></span> <span data-ttu-id="cab58-116">Wenn Sie chronologisch sortieren, finden Sie keine Zwischensummen.</span><span class="sxs-lookup"><span data-stu-id="cab58-116">If you sort chronologically, you will not see subtotals.</span></span>|  
    |<span data-ttu-id="cab58-117">**Layout**</span><span class="sxs-lookup"><span data-stu-id="cab58-117">**Layout**</span></span>|<span data-ttu-id="cab58-118">Gibt die Nummer des Berichtslayouts an.</span><span class="sxs-lookup"><span data-stu-id="cab58-118">Specifies the layout of the report.</span></span><br /><br /> <span data-ttu-id="cab58-119">Die Ergebnisse können in den folgenden Layouts angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="cab58-119">The results can be displayed in the following layouts:</span></span><br /><br /> <span data-ttu-id="cab58-120">**Standard**</span><span class="sxs-lookup"><span data-stu-id="cab58-120">**Standard**</span></span><br /> <span data-ttu-id="cab58-121">Zeigt die Kreditorennummer und den Kreditorennamen, zusammen mit den Buchungsdetails wie Dokumentennummer und den Betrag in lokaler Währung an.</span><span class="sxs-lookup"><span data-stu-id="cab58-121">Displays the vendor number and vendor name, together with posting details, such as the document number and the amount in local currency.</span></span><br /><br /> <span data-ttu-id="cab58-122">**FCY-Beträge**</span><span class="sxs-lookup"><span data-stu-id="cab58-122">**FCY Amounts**</span></span><br /> <span data-ttu-id="cab58-123">Zeigt die Kreditorennummer, Kreditorennamen, Belegnummer, Zahlungsstatus (O für den Wert Offen, PP. für Teilzahlung und C für geschlossene) an.</span><span class="sxs-lookup"><span data-stu-id="cab58-123">Displays the vendor number, vendor name, document number, payment status (O for open, PP for partial payment, and C for closed), and payment amount.</span></span><br /><br /> <span data-ttu-id="cab58-124">**Buchungsinfo**</span><span class="sxs-lookup"><span data-stu-id="cab58-124">**Posting Info**</span></span><br /> <span data-ttu-id="cab58-125">Zeigt die Kreditorennummer, den Kreditorennamen, die Kostenstelle, das Kostenobjekt, die Benutzer-ID und den Zahlungsbetrag an.</span><span class="sxs-lookup"><span data-stu-id="cab58-125">Displays the vendor number, vendor name, cost center, cost object, user ID, and payment amount.</span></span>|  

 <span data-ttu-id="cab58-126">Am Ende des Berichts wir die Anzahl der verarbeiteten Zahlungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cab58-126">At the end of the report, the number of processed payments is displayed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cab58-127">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cab58-127">See Also</span></span>  
[<span data-ttu-id="cab58-128">Zahlungen vornehmen</span><span class="sxs-lookup"><span data-stu-id="cab58-128">Making Payments</span></span>](../../payables-make-payments.md)
