---
title: Lieferbenachrichtigungen
description: Lieferbenachrichtigungen dienen dazu, überfällige Kreditorlieferungen zu verfolgen und Kreditoren an überfällige Lieferungen zu erinnern.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: b9751971d18821a57a28e553adcc4be2e844a295
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778716"
---
# <a name="delivery-reminders"></a><span data-ttu-id="6c078-103">Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="6c078-103">Delivery Reminders</span></span>
<span data-ttu-id="6c078-104">Lieferbenachrichtigungen dienen dazu, überfällige Kreditorlieferungen zu verfolgen und Kreditoren an überfällige Lieferungen zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="6c078-104">Delivery reminders are used to track overdue vendor shipments and to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="6c078-105">Zur Erstellung von Lieferbenachrichtigungen müssen Sie Folgendes einrichten:</span><span class="sxs-lookup"><span data-stu-id="6c078-105">To create delivery reminders, you must set up the following:</span></span>  

- <span data-ttu-id="6c078-106">Lieferbenachrichtigungsmethoden</span><span class="sxs-lookup"><span data-stu-id="6c078-106">Delivery reminder terms</span></span>  

    <span data-ttu-id="6c078-107">Lieferbenachrichtigungsmethoden werden durch einen Code identifiziert, der Kreditoren zugewiesen werden muss.</span><span class="sxs-lookup"><span data-stu-id="6c078-107">Delivery reminder terms are identified by a code that must be assigned to vendors.</span></span> <span data-ttu-id="6c078-108">Um mehrere Einstellungskombinationen verwenden zu können, müssen Sie jeweils für jede Einstellung getrennt einen Code festlegen.</span><span class="sxs-lookup"><span data-stu-id="6c078-108">To use more than one combination of settings, you must set up a code for each setting separately.</span></span> <span data-ttu-id="6c078-109">Sie können eine beliebige Anzahl an Lieferbenachrichtigungsmethoden einrichten.</span><span class="sxs-lookup"><span data-stu-id="6c078-109">You can set up any number of delivery reminder terms.</span></span>  

- <span data-ttu-id="6c078-110">Lieferbenachrichtigungsstufen</span><span class="sxs-lookup"><span data-stu-id="6c078-110">Delivery reminder levels</span></span>  

    <span data-ttu-id="6c078-111">Für jede Lieferbenachrichtigungsmethode müssen gesonderte Lieferbenachrichtigungstexte festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6c078-111">For every delivery reminder term, you must set up delivery reminder levels.</span></span> <span data-ttu-id="6c078-112">Diese Stufen bestimmen, wie oft Lieferbenachrichtigungen für eine bestimmte Methode erzeugt werden können.</span><span class="sxs-lookup"><span data-stu-id="6c078-112">These levels determine how often delivery reminders can be created for a specific term.</span></span> <span data-ttu-id="6c078-113">Stufe 1 ist die erste Lieferbenachrichtigung, die Sie für eine überfällige Lieferung erstellen.</span><span class="sxs-lookup"><span data-stu-id="6c078-113">Level 1 is the first delivery reminder that you create for an overdue delivery.</span></span> <span data-ttu-id="6c078-114">Stufe 2 ist die zweite Lieferbenachrichtigung und so weiter.</span><span class="sxs-lookup"><span data-stu-id="6c078-114">Level 2 is the second delivery reminder, and so on.</span></span> <span data-ttu-id="6c078-115">Bei der Erstellung von Lieferbenachrichtigungen wird die Anzahl der zuvor erstellten Benachrichtigungen berücksichtigt und die für die aktuelle Anzahl definierte Methode verwendet.</span><span class="sxs-lookup"><span data-stu-id="6c078-115">When delivery reminders are created, the number of reminders that were created previously is considered, and the current number is used to apply terms.</span></span>  

- <span data-ttu-id="6c078-116">Lieferbenachrichtigungstexte</span><span class="sxs-lookup"><span data-stu-id="6c078-116">Delivery reminder texts messages</span></span>  

    <span data-ttu-id="6c078-117">Sie müssen für jede Lieferbenachrichtigungsstufe gesonderte Lieferbenachrichtigungstexte festlegen.</span><span class="sxs-lookup"><span data-stu-id="6c078-117">You must set up delivery reminder text messages for every delivery reminder level.</span></span> <span data-ttu-id="6c078-118">Es gibt zwei Arten von Lieferbenachrichtigungstexten: Vortexte und Nachtexte.</span><span class="sxs-lookup"><span data-stu-id="6c078-118">There are two types of delivery reminder text messages: beginning and ending.</span></span> <span data-ttu-id="6c078-119">Der Vortext wird unter dem Kopf vor der Liste von Einträgen, die angemahnt werden, gedruckt.</span><span class="sxs-lookup"><span data-stu-id="6c078-119">The beginning text message is printed under the header section, before the list of entries that are marked for reminder.</span></span> <span data-ttu-id="6c078-120">Der Nachtext wird nach dieser Liste gedruckt.</span><span class="sxs-lookup"><span data-stu-id="6c078-120">The ending text message is printed after this list.</span></span>  

<span data-ttu-id="6c078-121">Weitere Informationen finden Sie unter [Vorgehensweise: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span><span class="sxs-lookup"><span data-stu-id="6c078-121">For more information, see [Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span></span>  

<span data-ttu-id="6c078-122">Nachdem Sie die Liefermethoden eingerichtet haben, müssen Sie den Kreditoren Lieferbenachrichtigungsmethodencodes zuweisen.</span><span class="sxs-lookup"><span data-stu-id="6c078-122">After you have set up the delivery terms, you must assign the delivery reminder term codes to vendors.</span></span> <span data-ttu-id="6c078-123">Weitere Informationen finden Sie unter [Vorgehensweise: Zuweisen von Lieferbenachrichtigungen zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="6c078-123">For more information, see [Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md).</span></span>  

<span data-ttu-id="6c078-124">Lieferbenachrichtigungen können manuell oder automatisch erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6c078-124">You can create delivery reminders manually or automatically.</span></span> <span data-ttu-id="6c078-125">Sie können den Batchauftrag **Lieferbenachrichtigung erstellen** zum automatischen Erstellen von Lieferbenachrichtigungen nutzen.</span><span class="sxs-lookup"><span data-stu-id="6c078-125">You can use the **Create Delivery Reminder** batch job to create delivery reminders automatically.</span></span> <span data-ttu-id="6c078-126">Bei Verwendung dieses Batchauftrags können Sie die Bestellungen auswählen, für die Lieferbenachrichtigungen erstellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="6c078-126">This batch job allows you to select the purchase orders for which delivery reminders must be created.</span></span> <span data-ttu-id="6c078-127">Weitere Informationen finden Sie unter [Lieferbenachrichtigungen erstellen](how-to-issue-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="6c078-127">For more information, see [Generate Delivery Reminders](how-to-issue-delivery-reminders.md).</span></span>  

<span data-ttu-id="6c078-128">Sie können Dokumente auch in Bezug auf Bestell- oder Auftragspositionen verfolgen.</span><span class="sxs-lookup"><span data-stu-id="6c078-128">You can also track documents in relation to purchase order lines and sales order lines.</span></span>  

[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="6c078-129">stellt die folgenden Berichte bereit:</span><span class="sxs-lookup"><span data-stu-id="6c078-129">provides the following reports:</span></span>  

- <span data-ttu-id="6c078-130">**Reg. Lieferbenachrichtigung** – Zum Anzeigen der Lieferbenachrichtigungen für Kreditoren.</span><span class="sxs-lookup"><span data-stu-id="6c078-130">**Issued Delivery Reminder** - To view the delivery reminders for vendors.</span></span>  
- <span data-ttu-id="6c078-131">**Lieferbenachrichtigung - Test** - Zum Überprüfen der Lieferbenachrichtigungen vor deren Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="6c078-131">**Delivery Reminder - Test** - To verify the delivery reminders before you issue them.</span></span>  

<span data-ttu-id="6c078-132">Weitere Informationen finden Sie unter [Vorgehensweise: Drucken von Testberichten für  Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="6c078-132">For more information, see [Print Test Reports for Delivery Reminders](how-to-print-test-reports-for-delivery-reminders.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="6c078-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6c078-133">See Also</span></span>  
 <span data-ttu-id="6c078-134">[Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-134">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="6c078-135">[Einrichten von Lieferbenachrichtigungsbestimmungen, Stufen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-135">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="6c078-136">[So werden Lieferbenachrichtigungscodes zu Kreditoren zugewiesen](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-136">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="6c078-137">[So erstellen Sie Lieferanmahnungen](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-137">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 <span data-ttu-id="6c078-138">[So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-138">[Create Delivery Reminders Manually](how-to-create-delivery-reminders-manually.md) </span></span>  
 <span data-ttu-id="6c078-139">[Lieferbenachrichtigung registrieren](how-to-issue-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="6c078-139">[Issue Delivery Reminders](how-to-issue-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="6c078-140">So drucken Sie Testberichte vor dem Registrieren von Lieferanmahnungen</span><span class="sxs-lookup"><span data-stu-id="6c078-140">Print Test Reports for Delivery Reminders</span></span>](how-to-print-test-reports-for-delivery-reminders.md)
