---
title: 'Gewusst wie: Einrichten von Lieferbenachrichtigungen'
description: In Business Central können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/23/2020
ms.author: edupont
ms.openlocfilehash: 1485ba92600602df7c0a852a91c9232fb31edd87
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778684"
---
# <a name="set-up-delivery-reminders"></a><span data-ttu-id="25732-103">Gewusst wie: Einrichten von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="25732-103">Set Up Delivery Reminders</span></span>

<span data-ttu-id="25732-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen.</span><span class="sxs-lookup"><span data-stu-id="25732-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="25732-105">Um Lieferanmahnungen für Kreditoren zu erstellen, müssen Sie die Stammdaten für die Erstellung von Lieferanmahnungen sowie die Nummernserien für die Lieferanmahnungen auf der Seite **Kreditoren & Einkauf einrichten** einrichten.</span><span class="sxs-lookup"><span data-stu-id="25732-105">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders on the **Purchases & Payables Setup** page.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="25732-106">Gewusst wie: Einrichten von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="25732-106">To set up delivery reminders</span></span>  

1. <span data-ttu-id="25732-107">Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](../../media/ui-search/search_small.png "Tell me-Funktion"), geben Sie **Einrichten von Einkäufen und Verbindlichkeiten** ein, und wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="25732-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="25732-108">Geben Sie im Feld **Standard Lief.-Mahn. Datumsfeld** eine der Optionen an, wie in der folgenden Tabelle beschrieben.</span><span class="sxs-lookup"><span data-stu-id="25732-108">In the **Default Del. Rem. Date Field** field, specify one of the options described in the following table.</span></span>  

    |<span data-ttu-id="25732-109">Option</span><span class="sxs-lookup"><span data-stu-id="25732-109">Option</span></span>|<span data-ttu-id="25732-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25732-110">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="25732-111">**Gewünschtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="25732-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="25732-112">Gibt an, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="25732-112">Specifies that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="25732-113">**Zugesagtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="25732-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="25732-114">Gibt an, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="25732-114">Specifies that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="25732-115">**Erwartetes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="25732-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="25732-116">Gibt an, dass der Datumswert im Feld **Erwartetes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="25732-116">Specifies that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3. <span data-ttu-id="25732-117">Füllen Sie zusätzliche Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="25732-117">Fill in additional fields as described in the following table.</span></span>  

    |<span data-ttu-id="25732-118">Feld</span><span class="sxs-lookup"><span data-stu-id="25732-118">Field</span></span>|<span data-ttu-id="25732-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25732-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="25732-120">**Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="25732-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="25732-121">Der Nummernseriencode für Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="25732-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="25732-122">**Reg. Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="25732-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="25732-123">Der Nummernseriencode für ausgegebene Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="25732-123">The number series code for issued delivery reminders.</span></span>|  

4. <span data-ttu-id="25732-124">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="25732-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="25732-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="25732-125">See Also</span></span>

 <span data-ttu-id="25732-126">[Lieferanmahnungen](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="25732-126">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="25732-127">[Einrichten von Lieferbenachrichtigungsbestimmungen, Stufen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="25732-127">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 [<span data-ttu-id="25732-128">So werden Lieferbenachrichtigungscodes zu Kreditoren zugewiesen</span><span class="sxs-lookup"><span data-stu-id="25732-128">Assign Delivery Reminder Codes to Vendors</span></span>](how-to-assign-delivery-reminder-codes-to-vendors.md)  
 [<span data-ttu-id="25732-129">So erstellen Sie Lieferanmahnungen manuell</span><span class="sxs-lookup"><span data-stu-id="25732-129">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)
