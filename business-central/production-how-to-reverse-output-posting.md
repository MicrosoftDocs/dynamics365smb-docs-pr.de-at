---
title: 'Vorgehensweise: Ausgangsbuchung stornieren | Microsoft Docs'
description: Es kann vorkommen, dass die Buchung einer fertig gestellten Menge storniert werden muss. Dies ist z. B. der Fall, wenn eine fehlerhafte Dateneingabe passiert ist und eine falsche fertiggestellte Menge in einem Fertigungsauftrag gebucht wurde.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: fb107d6d165ede233799ab165d735c030c0c8bba
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/08/2019
ms.locfileid: "823512"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="9eeeb-104">Gebuchte fertig gestellte Menge stornieren</span><span class="sxs-lookup"><span data-stu-id="9eeeb-104">Reverse Output Posting</span></span>
<span data-ttu-id="9eeeb-105">Es kann vorkommen, dass die Buchung einer fertig gestellten Menge storniert werden muss.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="9eeeb-106">Dies ist z. B. der Fall, wenn eine fehlerhafte Dateneingabe passiert ist und eine falsche fertiggestellte Menge in einem Fertigungsauftrag gebucht wurde.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="9eeeb-107">Eine Ausgangsbuchung stornieren</span><span class="sxs-lookup"><span data-stu-id="9eeeb-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="9eeeb-108">Wählen Sie das Symbol ![Glühlampe, mit der die Funktion „Wie möchten Sie weiter verfahren“ geöffnet wird](media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") aus, geben Sie **Artikel Ausgabe-Buch.-Blätter** ein, und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="9eeeb-109">Wählen Sie Ihren Stapel aus.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-109">Select your batch.</span></span>  
2. <span data-ttu-id="9eeeb-110">Füllen Sie die Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="9eeeb-111">Weitere Informationen finden Sie unter [Produktionsausgabe und Laufzeiten über Stapelverarbeitung buchen](production-how-to-post-output-quantity.md)</span><span class="sxs-lookup"><span data-stu-id="9eeeb-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="9eeeb-112">Wählen Sie im Feld **Ausgleich mit Lfd. Nr.** den zugeordneten Artikelposten aus.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="9eeeb-113">Dadurch werden der Kapazitäts- und der Artikelposten storniert.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="9eeeb-114">Buchen Sie die Stornierung, indem Sie das Buch.-Blatt buchen.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="9eeeb-115">Die Posten im FA-Istmeldungsprotokoll werden im Hauptartikelposten als positiver Ausgleich gebucht.</span><span class="sxs-lookup"><span data-stu-id="9eeeb-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9eeeb-116">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9eeeb-116">See Also</span></span>  
 <span data-ttu-id="9eeeb-117">[Produktion](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="9eeeb-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="9eeeb-118">Produktion einrichten</span><span class="sxs-lookup"><span data-stu-id="9eeeb-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="9eeeb-119">[Planung](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="9eeeb-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="9eeeb-120">Lagerbesttand</span><span class="sxs-lookup"><span data-stu-id="9eeeb-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="9eeeb-121">Einkauf</span><span class="sxs-lookup"><span data-stu-id="9eeeb-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="9eeeb-122">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9eeeb-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
