---
title: "Vorgehensweise: Schließen von offenen Artikelposten aus einem festen Ausgleich im Artikel Buch.-Blatt | Microsoft Docs"
description: "Sie können das Feld **Ausgegl. von Posten** auf der Seite **Artikel Buch.-Blatt** verwenden, um einen festen Ausgleich zwischen einer eingehenden Transaktion und der ursprünglichen ausgehenden Transaktion zu erstellen. Beispielsweise um die ausgehende Transaktion zu korrigieren oder ihre Rückgabe zu verarbeiten."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: e3f210b86168d34ec775f85b416b6d0e365cce88
ms.contentlocale: de-at
ms.lasthandoff: 11/26/2018

---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="1da9d-104">Schließen von offenen Artikelposten aus einem festen Ausgleich im Artikel Buch.-Blatt</span><span class="sxs-lookup"><span data-stu-id="1da9d-104">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>
<span data-ttu-id="1da9d-105">Sie können das Feld **Ausgegl. von Posten** auf der Seite **Artikel Buch.-Blatt** verwenden, um einen festen Ausgleich zwischen einer eingehenden Transaktion und der ursprünglichen ausgehenden Transaktion zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-105">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="1da9d-106">Beispielsweise um die ausgehende Transaktion zu korrigieren oder ihre Rückgabe zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="1da9d-106">For example, to correct the outbound transaction or to process its return.</span></span> <span data-ttu-id="1da9d-107">Weitere Informationen finden Sie unter Ausgegl. von Posten.</span><span class="sxs-lookup"><span data-stu-id="1da9d-107">For more information, see Applies-from Entry.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="1da9d-108">Feste Ausgleiche, die auf diese Weise vorgenommen werden, gelten nur für die Kosten, nicht für die Menge.</span><span class="sxs-lookup"><span data-stu-id="1da9d-108">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="1da9d-109">Entsprechend schließt der gebuchte positive Artikelposten nicht den angewendeten ausgehenden Posten und bleibt selbst offen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="1da9d-110">Dies gilt auch, wenn Sie einen festen Ausgleich für einen positiven Posten mit einem negativen Posten buchen, der nicht durch einen positiven regulären Posten geschlossen wurde. Dann bleiben die positiven und negativen Posten offen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>   
>  <span data-ttu-id="1da9d-111">Dies bedeutet auch, dass Sie eine Lagerbuchungsperiode nicht schließen können, wenn ein solcher Posten vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="1da9d-111">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="1da9d-112">Der folgende Ablauf zeigt, wie solche Posten durch Ausführen von zwei korrigierenden Buchungen im Artikel Buch.-Blatt geschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="1da9d-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="1da9d-113">So schließen Sie offene Artikelposten, die aus einem festen Ausgleich im Artikel Buch.-Blatt entstanden sind</span><span class="sxs-lookup"><span data-stu-id="1da9d-113">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1.  <span data-ttu-id="1da9d-114">Verwenden Sie das Feld **Ausgegl. von Posten**, um einen Zugang mit der entsprechenden Menge zu buchen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="1da9d-115">Dadurch wird der ursprüngliche negative Posten mit einem festen Ausgleich geschlossen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-115">This closes the original negative entry with a fixed application.</span></span>  
2.  <span data-ttu-id="1da9d-116">Verwenden Sie das Feld **Ausgegl. von Posten**, um einen Abgang zu buchen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="1da9d-117">Dadurch wird der ursprüngliche korrigierende positive Posten mit einem festen Ausgleich geschlossen.</span><span class="sxs-lookup"><span data-stu-id="1da9d-117">This closes the original corrective positive entry with a fixed application.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1da9d-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1da9d-118">See Also</span></span>  
[<span data-ttu-id="1da9d-119">Entfernen und erneutes Ausgleichen von Artikelposten</span><span class="sxs-lookup"><span data-stu-id="1da9d-119"> Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
 <span data-ttu-id="1da9d-120">[Verarbeiten von Verkaufsrücklieferung und Stornierungen](sales-how-process-sales-returns-cancellations.md) </span><span class="sxs-lookup"><span data-stu-id="1da9d-120">[Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md) </span></span>  
 <span data-ttu-id="1da9d-121">[Einrichten der Lagerwertberechnung und der Kostenrechnung](finance-set-up-inventory-valuation-and-costing.md) </span><span class="sxs-lookup"><span data-stu-id="1da9d-121">[Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md) </span></span>  
 <span data-ttu-id="1da9d-122">[Verwalten der Lagerregulierung](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="1da9d-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 [<span data-ttu-id="1da9d-123">Designdetails: Kostenberechnungsmethoden</span><span class="sxs-lookup"><span data-stu-id="1da9d-123">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)

