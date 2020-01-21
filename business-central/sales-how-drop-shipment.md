---
title: Erstellen Sie einen Verkaufsauftrag, der mit einer Einkaufsbestellung für eine direkte Lieferung verknüpft ist | Microsoft Docs
description: Beschreibt, wie Sie einen Verkaufsauftrag erstellen, der mit einer Bestellung verknüpft ist, um sicherzustellen, dass die Artikel vom Kreditor direkt an den Debitor versendet werden
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 50198afaa8caae9a11a06a25357fa94ad26b0b8f
ms.sourcegitcommit: b570997f93d1f7141bc9539c93a67a91226660a8
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 01/08/2020
ms.locfileid: "2943202"
---
# <a name="make-drop-shipments"></a><span data-ttu-id="5ad86-103">Direktlieferungen machen</span><span class="sxs-lookup"><span data-stu-id="5ad86-103">Make Drop Shipments</span></span>
<span data-ttu-id="5ad86-104">Eine Direktlieferung ist die Lieferung von Artikeln, von einem Ihrer Kreditoren direkt an einen Ihrer Debitoren.</span><span class="sxs-lookup"><span data-stu-id="5ad86-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="5ad86-105">Wenn ein Verkaufsauftrag für die Direktlieferung markiert ist und Sie einen Verkaufsauftrag erstellen, bei dem der Kunde im **Lief. an**-Feld, **Adresse Debitor** angegeben ist, können Sie die beiden Dokumente verknüpfen und so den Lieferanten anweisen, direkt an den Kunden zu senden.</span><span class="sxs-lookup"><span data-stu-id="5ad86-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM]

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="5ad86-106">So erstellen Sie einen Verkaufsauftrag für eine Direktlieferung</span><span class="sxs-lookup"><span data-stu-id="5ad86-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="5ad86-107">Um eine Direktlieferung vorzubereiten, erstellen Sie einen normalen Verkaufsauftrag für einen Artikel, außer dass Sie in der Verkaufsauftragszeile angeben müssen, dass für den Verkauf Direktlieferung benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="5ad86-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="5ad86-108">Legen Sie einen Verkaufsauftrag für einen Artikel an.</span><span class="sxs-lookup"><span data-stu-id="5ad86-108">Create a sales order for an item.</span></span> <span data-ttu-id="5ad86-109">Weitere Informationen finden Sie unter [Produkte verkaufen](sales-how-sell-products.md)</span><span class="sxs-lookup"><span data-stu-id="5ad86-109">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="5ad86-110">Aktivieren Sie in der Verkaufsauftragszeile für den Direktlieferungsartikel das Kontrollkästchen **Direktlieferung**.</span><span class="sxs-lookup"><span data-stu-id="5ad86-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="5ad86-111">Verwenden Sie die Funktion **Spalten auswählen**, wenn das Feld nicht sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="5ad86-111">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="5ad86-112">Weitere Informationen finden Sie unter [Personalisieren Sie Ihren Arbeitsbereich](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="5ad86-112">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="5ad86-113">So erstellen Sie Bestellungen für Direktlieferungen:</span><span class="sxs-lookup"><span data-stu-id="5ad86-113">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="5ad86-114">Um eine Direktlieferung für den Artikel, der verkauft werden soll, vorzubereiten, erstellen Sie eine normale Bestellung, außer dass Sie in der Bestellung angeben müssen, dass direkt an den Debitoren geliefert wird, nicht an Sie selbst.</span><span class="sxs-lookup"><span data-stu-id="5ad86-114">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="5ad86-115">Erstellen Sie eine Bestellung.</span><span class="sxs-lookup"><span data-stu-id="5ad86-115">Create a purchase order.</span></span> <span data-ttu-id="5ad86-116">Füllen Sie keines dieser Felder in den Zeilen aus.</span><span class="sxs-lookup"><span data-stu-id="5ad86-116">Do not fill any fields on the lines.</span></span> <span data-ttu-id="5ad86-117">Weitere Informationen finden Sie unter [Erfassen eines Einkaufs](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="5ad86-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="5ad86-118">Wählen Sie im Feld **Lief. an** **Adresse Debitor** aus.</span><span class="sxs-lookup"><span data-stu-id="5ad86-118">In the **Ship-to** field, select **Customer Address**.</span></span>
3. <span data-ttu-id="5ad86-119">Wählen Sie im Feld **Debitor** den Debitor aus, an den Sie verkaufen.</span><span class="sxs-lookup"><span data-stu-id="5ad86-119">In the **Customer** field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="5ad86-120">Wählen Sie die Aktion **Direktlieferungen** aus, und dann die Aktion **Auftrag holen**.</span><span class="sxs-lookup"><span data-stu-id="5ad86-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="5ad86-121">Auf der Seite **Verkaufsübersicht** wählen Sie den Auftrag, den Sie im Abschnitt [So erstellen Sie einen Verkaufsauftrag für Direktlieferung](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment) vorbereitet haben.</span><span class="sxs-lookup"><span data-stu-id="5ad86-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span></span>
5. <span data-ttu-id="5ad86-122">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="5ad86-122">Choose the **OK** button.</span></span>

<span data-ttu-id="5ad86-123">Die Zeileninformation aus dem Auftrag werden in die Bestellzeile eingetragen.</span><span class="sxs-lookup"><span data-stu-id="5ad86-123">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="5ad86-124">Sie können nun den Kreditor anweisen, die Artikel an Ihren Kunden zu versenden, indem Sie ihm beispielsweise die Bestellung als PDF-Datei senden.</span><span class="sxs-lookup"><span data-stu-id="5ad86-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="5ad86-125">So zeigen Sie den verknüpften Auftrag aus der Bestellung an</span><span class="sxs-lookup"><span data-stu-id="5ad86-125">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="5ad86-126">Wählen Sie die Verkaufsauftragszeile der Direktlieferung aus, dann die Aktion **Bestellung**, die Aktion **Direktlieferung** und die Aktion **Bestellung**.</span><span class="sxs-lookup"><span data-stu-id="5ad86-126">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="5ad86-127">So buchen Sie eine Direktlieferung:</span><span class="sxs-lookup"><span data-stu-id="5ad86-127">To post a drop shipment</span></span>
<span data-ttu-id="5ad86-128">Wenn der Kreditor die Artikel geliefert hat, können Sie den Verkaufsauftrag als geliefert buchen.</span><span class="sxs-lookup"><span data-stu-id="5ad86-128">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="5ad86-129">Sie können auch die Bestellung buchen, aber nur mit der Option **Erhalten** bis der Verkaufsauftrag fakturiert wurde.</span><span class="sxs-lookup"><span data-stu-id="5ad86-129">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="5ad86-130">Wählen Sie die ![Glühbirne, die das Tell Me Feature](media/ui-search/search_small.png "Tell Me-Funktion") Symbol öffnet, geben Sie **Verkaufsaufträge** ein und wählen Sie dann den entsprechenden Link.</span><span class="sxs-lookup"><span data-stu-id="5ad86-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="5ad86-131">Öffnen Sie den Verkaufsauftrag, den Sie in [So erstellen Sie einen Verkaufsauftrag für Direktlieferung]() erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="5ad86-131">Open the sales order that you created in [To create a sales order for drop shipment]().</span></span>
3. <span data-ttu-id="5ad86-132">Geben Sie im Feld **Zu liefern** an, wieviele der Bestellmengen geliefert werden sollen, die gesamte Menge oder eine Teilmenge.</span><span class="sxs-lookup"><span data-stu-id="5ad86-132">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="5ad86-133">Wählen Sie die Aktion **Buchen** oder **Buchen und Senden** aus.</span><span class="sxs-lookup"><span data-stu-id="5ad86-133">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="5ad86-134">Wählen Sie dann entweder die Option **Liefern**, um zu einem späteren Zeitpunkt zu fakturieren oder **Liefern und Fakturieren**, um sofort zu fakturieren.</span><span class="sxs-lookup"><span data-stu-id="5ad86-134">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="5ad86-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5ad86-135">See Also</span></span>
[<span data-ttu-id="5ad86-136">Spezialaufträge erstellen:</span><span class="sxs-lookup"><span data-stu-id="5ad86-136">Create Special Orders</span></span>](sales-how-to-create-special-orders.md)  
[<span data-ttu-id="5ad86-137">Einkauf von Artikeln für einen Verkauf</span><span class="sxs-lookup"><span data-stu-id="5ad86-137">Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="5ad86-138">Produkte verkaufen</span><span class="sxs-lookup"><span data-stu-id="5ad86-138">Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="5ad86-139">Erfassen eines Einkaufs</span><span class="sxs-lookup"><span data-stu-id="5ad86-139">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="5ad86-140">Verkauf</span><span class="sxs-lookup"><span data-stu-id="5ad86-140">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="5ad86-141">Lagerbestand</span><span class="sxs-lookup"><span data-stu-id="5ad86-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="5ad86-142">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5ad86-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
