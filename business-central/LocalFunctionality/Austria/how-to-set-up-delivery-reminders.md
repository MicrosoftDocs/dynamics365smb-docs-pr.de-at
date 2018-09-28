---
title: 'Gewusst wie: Einrichten von Lieferbenachrichtigungen'
description: "In Business Central können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen."
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 3284b413303c745b230e37611f7a2a9b0061e1f9
ms.contentlocale: de-at
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-delivery-reminders"></a><span data-ttu-id="cbdf2-103">Gewusst wie: Einrichten von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="cbdf2-103">Set Up Delivery Reminders</span></span>
<span data-ttu-id="cbdf2-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] können Sie Lieferbenachrichtigungen nutzen, um Verkäufer über verspätete Lieferungen zu mahnen.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="cbdf2-105">Um Lieferanmahnungen für Kreditoren zu erstellen, müssen Sie die Stammdaten für die Erstellung von Lieferanmahnungen sowie die Nummernserien für die Lieferanmahnungen in dem Fenster **Kreditoren & Einkauf einrichten** einrichten.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-105">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders in the **Purchases & Payables Setup** window.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="cbdf2-106">Gewusst wie: Einrichten von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="cbdf2-106">To set up delivery reminders</span></span>  

1.  <span data-ttu-id="cbdf2-107">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht  suchen")und geben **Kreditoren- und Debitoren-Einrichtung** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cbdf2-108">Wählen Sie im Inforegister **Allgemein** im Feld **Standard ENTF. Abbau, AfA**, geben Sie eine der folgenden Optionen an, wie in der folgenden Tabelle beschrieben.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-108">On the **General** FastTab, in the **Default Del. Rem. Date Field** field, specify one of the following options as described in the following table.</span></span>  

    |<span data-ttu-id="cbdf2-109">Option</span><span class="sxs-lookup"><span data-stu-id="cbdf2-109">Option</span></span>|<span data-ttu-id="cbdf2-110">Description</span><span class="sxs-lookup"><span data-stu-id="cbdf2-110">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="cbdf2-111">**Gewünschtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="cbdf2-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="cbdf2-112">Um anzugeben, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-112">To specify that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="cbdf2-113">**Zugesagtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="cbdf2-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="cbdf2-114">Um anzugeben, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-114">To specify that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="cbdf2-115">**Erwartetes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="cbdf2-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="cbdf2-116">Um anzugeben, dass der Datumswert im Feld **Erwartetes Wareneingangsdatum** in der Bestellzeile als Standarddatum für die Erstellung von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-116">To specify that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3.  <span data-ttu-id="cbdf2-117">Füllen Sie im Inforegister **Nummerierung** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-117">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cbdf2-118">Feld</span><span class="sxs-lookup"><span data-stu-id="cbdf2-118">Field</span></span>|<span data-ttu-id="cbdf2-119">Description</span><span class="sxs-lookup"><span data-stu-id="cbdf2-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cbdf2-120">**Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="cbdf2-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="cbdf2-121">Der Nummernseriencode für Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="cbdf2-122">**Reg. Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="cbdf2-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="cbdf2-123">Der Nummernseriencode für ausgegebene Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-123">The number series code for issued delivery reminders.</span></span>|  

4.  <span data-ttu-id="cbdf2-124">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="cbdf2-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cbdf2-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cbdf2-125">See Also</span></span>  
 <span data-ttu-id="cbdf2-126">[Lieferanmahnungen](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="cbdf2-126">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="cbdf2-127">[Einrichten von Lieferbenachrichtigungsbestimmungen, Stufen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="cbdf2-127">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="cbdf2-128">[So werden Lieferbenachrichtigungscodes zu Kreditoren zugewiesen](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="cbdf2-128">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 [<span data-ttu-id="cbdf2-129">So erstellen Sie Lieferanmahnungen manuell</span><span class="sxs-lookup"><span data-stu-id="cbdf2-129">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)

