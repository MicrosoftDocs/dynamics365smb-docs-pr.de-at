---
title: 'Vorgehensweise: Schließen von offenen Artikelposten aus einem festen Ausgleich im Artikel Buch.-Blatt | Microsoft Docs'
description: Sie können das Feld **Ausgegl. von Posten** auf der Seite **Artikel Buch.-Blatt** verwenden, um einen festen Ausgleich zwischen einer eingehenden Transaktion und der ursprünglichen ausgehenden Transaktion zu erstellen. Beispielsweise um die ausgehende Transaktion zu korrigieren oder ihre Rückgabe zu verarbeiten.
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
ms.openlocfilehash: e3f210b86168d34ec775f85b416b6d0e365cce88
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/08/2019
ms.locfileid: "823694"
---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="bb32c-104">Schließen von offenen Artikelposten aus einem festen Ausgleich im Artikel Buch.-Blatt</span><span class="sxs-lookup"><span data-stu-id="bb32c-104">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>
<span data-ttu-id="bb32c-105">Sie können das Feld **Ausgegl. von Posten** auf der Seite **Artikel Buch.-Blatt** verwenden, um einen festen Ausgleich zwischen einer eingehenden Transaktion und der ursprünglichen ausgehenden Transaktion zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-105">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="bb32c-106">Beispielsweise um die ausgehende Transaktion zu korrigieren oder ihre Rückgabe zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="bb32c-106">For example, to correct the outbound transaction or to process its return.</span></span> <span data-ttu-id="bb32c-107">Weitere Informationen finden Sie unter Ausgegl. von Posten.</span><span class="sxs-lookup"><span data-stu-id="bb32c-107">For more information, see Applies-from Entry.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="bb32c-108">Feste Ausgleiche, die auf diese Weise vorgenommen werden, gelten nur für die Kosten, nicht für die Menge.</span><span class="sxs-lookup"><span data-stu-id="bb32c-108">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="bb32c-109">Entsprechend schließt der gebuchte positive Artikelposten nicht den angewendeten ausgehenden Posten und bleibt selbst offen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="bb32c-110">Dies gilt auch, wenn Sie einen festen Ausgleich für einen positiven Posten mit einem negativen Posten buchen, der nicht durch einen positiven regulären Posten geschlossen wurde. Dann bleiben die positiven und negativen Posten offen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>   
>  <span data-ttu-id="bb32c-111">Dies bedeutet auch, dass Sie eine Lagerbuchungsperiode nicht schließen können, wenn ein solcher Posten vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="bb32c-111">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="bb32c-112">Der folgende Ablauf zeigt, wie solche Posten durch Ausführen von zwei korrigierenden Buchungen im Artikel Buch.-Blatt geschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="bb32c-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="bb32c-113">So schließen Sie offene Artikelposten, die aus einem festen Ausgleich im Artikel Buch.-Blatt entstanden sind</span><span class="sxs-lookup"><span data-stu-id="bb32c-113">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1.  <span data-ttu-id="bb32c-114">Verwenden Sie das Feld **Ausgegl. von Posten**, um einen Zugang mit der entsprechenden Menge zu buchen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="bb32c-115">Dadurch wird der ursprüngliche negative Posten mit einem festen Ausgleich geschlossen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-115">This closes the original negative entry with a fixed application.</span></span>  
2.  <span data-ttu-id="bb32c-116">Verwenden Sie das Feld **Ausgegl. von Posten**, um einen Abgang zu buchen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="bb32c-117">Dadurch wird der ursprüngliche korrigierende positive Posten mit einem festen Ausgleich geschlossen.</span><span class="sxs-lookup"><span data-stu-id="bb32c-117">This closes the original corrective positive entry with a fixed application.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bb32c-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="bb32c-118">See Also</span></span>  
[<span data-ttu-id="bb32c-119">Entfernen und erneutes Ausgleichen von Artikelposten</span><span class="sxs-lookup"><span data-stu-id="bb32c-119"> Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
 <span data-ttu-id="bb32c-120">[Verarbeiten von Verkaufsrücklieferung und Stornierungen](sales-how-process-sales-returns-cancellations.md) </span><span class="sxs-lookup"><span data-stu-id="bb32c-120">[Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md) </span></span>  
 <span data-ttu-id="bb32c-121">[Einrichten der Lagerwertberechnung und der Kostenrechnung](finance-set-up-inventory-valuation-and-costing.md) </span><span class="sxs-lookup"><span data-stu-id="bb32c-121">[Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md) </span></span>  
 <span data-ttu-id="bb32c-122">[Verwalten der Lagerregulierung](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="bb32c-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 [<span data-ttu-id="bb32c-123">Designdetails: Kostenberechnungsmethoden</span><span class="sxs-lookup"><span data-stu-id="bb32c-123">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)
