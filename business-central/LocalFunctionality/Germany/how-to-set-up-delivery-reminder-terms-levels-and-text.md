---
title: 'Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, -stufen und -text'
description: "Zur Erstellung von Lieferbenachrichtigungen müssen Sie bestimmte Dinge einrichten."
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
ms.openlocfilehash: e5e7c699cb743b1a45780005d1429a1baf93f716
ms.contentlocale: de-at
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-delivery-reminder-terms-levels-and-text"></a><span data-ttu-id="be567-103">Einrichten von Lieferbenachrichtigungsbestimmungen, Stufen und Text</span><span class="sxs-lookup"><span data-stu-id="be567-103">Set Up Delivery Reminder Terms, Levels, and Text</span></span>
<span data-ttu-id="be567-104">Zur Erstellung von Lieferbenachrichtigungen müssen Sie Folgendes einrichten:</span><span class="sxs-lookup"><span data-stu-id="be567-104">To create delivery reminders, you must set up the following:</span></span>  

- <span data-ttu-id="be567-105">Lieferbenachrichtigungsmethoden</span><span class="sxs-lookup"><span data-stu-id="be567-105">Delivery reminder terms</span></span>  
- <span data-ttu-id="be567-106">Lieferbenachrichtigungsstufen</span><span class="sxs-lookup"><span data-stu-id="be567-106">Delivery reminder levels</span></span>  
- <span data-ttu-id="be567-107">Lieferbenachrichtigungstexte</span><span class="sxs-lookup"><span data-stu-id="be567-107">Delivery reminder text messages</span></span>  

<span data-ttu-id="be567-108">Jede Lieferbenachrichtigungsmethoden verfügt über mindestens zwei Lieferbenachrichtigungsstufe und für jede Lieferbenachrichtigungsstufe können Sie Text angeben, der in die Lieferbenachrichtigung aufgenommen wird.</span><span class="sxs-lookup"><span data-stu-id="be567-108">Each delivery reminder term has two or more delivery reminder levels, and for each delivery reminder level, you can specify text that will be part of the delivery reminder.</span></span>  

<span data-ttu-id="be567-109">Weitere Informationen finden Sie unter [Lieferbenachrichtigungen](delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="be567-109">For more information, see [Delivery Reminders](delivery-reminders.md).</span></span>  

## <a name="to-set-up-delivery-reminder-terms"></a><span data-ttu-id="be567-110">So richten Sie Lieferbenachrichtigungsmethoden ein</span><span class="sxs-lookup"><span data-stu-id="be567-110">To set up delivery reminder terms</span></span>  

1.  <span data-ttu-id="be567-111">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), geben Sie **Lieferbenachrichtigungsmethoden** ein, und wählen Sie dann den zugehörigen Link.</span><span class="sxs-lookup"><span data-stu-id="be567-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delivery Reminder Terms**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="be567-112">Wählen Sie die Aktion **Neu**.</span><span class="sxs-lookup"><span data-stu-id="be567-112">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="be567-113">Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="be567-113">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="be567-114">Feld</span><span class="sxs-lookup"><span data-stu-id="be567-114">Field</span></span>|<span data-ttu-id="be567-115">Description</span><span class="sxs-lookup"><span data-stu-id="be567-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="be567-116">**Code**</span><span class="sxs-lookup"><span data-stu-id="be567-116">**Code**</span></span>|<span data-ttu-id="be567-117">Der Code für die Lieferbenachrichtigungsmethode.</span><span class="sxs-lookup"><span data-stu-id="be567-117">The code for the delivery reminder term.</span></span> <span data-ttu-id="be567-118">Sie können bis zu 10 alphanumerische Zeichen eingeben.</span><span class="sxs-lookup"><span data-stu-id="be567-118">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="be567-119">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="be567-119">**Description**</span></span>|<span data-ttu-id="be567-120">Der Beschreibung für die Lieferbenachrichtigungsmethode.</span><span class="sxs-lookup"><span data-stu-id="be567-120">The description for the delivery reminder term.</span></span> <span data-ttu-id="be567-121">Sie können bis zu 30 alphanumerische Zeichen eingeben.</span><span class="sxs-lookup"><span data-stu-id="be567-121">You can enter a maximum of 30 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="be567-122">**Max. Anzahl Lieferbenachrichtigungen**</span><span class="sxs-lookup"><span data-stu-id="be567-122">**Max. No. of Delivery Reminders**</span></span>|<span data-ttu-id="be567-123">Die maximale Anzahl von Lieferbenachrichtigungen, die für eine Bestellung erstellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="be567-123">The maximum number of delivery reminders that can be created for an order.</span></span><br /><br /> <span data-ttu-id="be567-124">**HINWEIS:** Diese Höchstgrenze gilt für alle Benachrichtigungsstufen dieser Benachrichtigungsmethode zusammen.</span><span class="sxs-lookup"><span data-stu-id="be567-124">**NOTE:** This is the maximum number across all reminder levels for this reminder term.</span></span> <span data-ttu-id="be567-125">Wenn Sie z. B. drei Stufen definiert haben und **Max. Anzahl Lieferbenachrichtigungen** auf 5 festlegen, wird die erste Mahnung auf Stufe 1, die Zweite auf Stufe 2, die Dritte auf Stufe 3 erstellt.</span><span class="sxs-lookup"><span data-stu-id="be567-125">For example, if you have set up three levels, and you set **Max. No. of Delivery Reminders** to 5, the first reminder is created at level 1, the second at level 2, and the last three at level 3.</span></span>|  

4.  <span data-ttu-id="be567-126">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="be567-126">Choose the **OK** button.</span></span>  

## <a name="to-add-delivery-reminder-levels-to-a-delivery-reminder-term"></a><span data-ttu-id="be567-127">So fügen Sie einer Lieferanmahnungsmethode Lieferanmahnungsstufen hinzu</span><span class="sxs-lookup"><span data-stu-id="be567-127">To add delivery reminder levels to a delivery reminder term</span></span>  

1.  <span data-ttu-id="be567-128">Wählen Sie im Fenster **Lieferbenachrichtigungsmethoden** die Lieferbenachrichtigung aus, der Sie Stufen hinzufügen möchten, und wählen Sie dann die Aktion **Bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="be567-128">In the **Delivery Reminder Terms** window, select the delivery reminder term for which you want to set up levels, and then choose the **Levels** action.</span></span>  
2.  <span data-ttu-id="be567-129">Wählen Sie die Aktion **Neu**.</span><span class="sxs-lookup"><span data-stu-id="be567-129">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="be567-130">Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="be567-130">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="be567-131">Feld</span><span class="sxs-lookup"><span data-stu-id="be567-131">Field</span></span>|<span data-ttu-id="be567-132">Description</span><span class="sxs-lookup"><span data-stu-id="be567-132">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="be567-133">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="be567-133">**No.**</span></span>|<span data-ttu-id="be567-134">Die Nummer der Lieferbenachrichtigungsstufe.</span><span class="sxs-lookup"><span data-stu-id="be567-134">The delivery reminder level number.</span></span> <span data-ttu-id="be567-135">Dieses Feld wird automatisch ausgefüllt.</span><span class="sxs-lookup"><span data-stu-id="be567-135">This field is filled in automatically.</span></span>|  
    |<span data-ttu-id="be567-136">**Berechnung Fälligkeitsdatum**</span><span class="sxs-lookup"><span data-stu-id="be567-136">**Due Date Calculation**</span></span>|<span data-ttu-id="be567-137">Die Formel für die Fälligkeitsdatumsberechnung der Lieferbenachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="be567-137">The formula for the due date calculation for the delivery reminder.</span></span> <span data-ttu-id="be567-138">Sie können eine Kombination von Zahlen zwischen 0 und 9999 sowie Datumscodes (T für Tag, WT für Wochentag, W für Woche, M für Monat, Q für Quartal oder J für Jahr) eingeben.</span><span class="sxs-lookup"><span data-stu-id="be567-138">You can enter a combination of numbers from 0 to 9999, and date codes (D for day, WD for weekday, W for week, M for month, Q for quarter, or Y for year).</span></span> <span data-ttu-id="be567-139">Die Datumscodes bezeichnen die Berechnung desFälligkeitsdatums der Lieferbenachrichtigung fest.</span><span class="sxs-lookup"><span data-stu-id="be567-139">The date codes denote the calculation for the delivery reminder due date.</span></span> <span data-ttu-id="be567-140">Sie können bis zu 20 Zeichen für die Berechnungsformel für den Fälligkeitstermin eingeben.</span><span class="sxs-lookup"><span data-stu-id="be567-140">You can enter a maximum of 20 characters for the due date calculation formula.</span></span>|  

4.  <span data-ttu-id="be567-141">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="be567-141">Choose the **OK** button.</span></span>  

<span data-ttu-id="be567-142">Für jede Lieferbenachrichtigungsstufe können Sie Textnachrichtigen definieren, die der Lieferbenachrichtigung hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="be567-142">For each delivery reminder level, you can define text messages that are added to the delivery reminder.</span></span> <span data-ttu-id="be567-143">Sie können Vortext definieren, der vor der Beschreibung der überfälligen Bestellung eingefügt wird, und Nachtext, der nach der Beschreibung der überfälligen Bestellung eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="be567-143">You can define beginning text that is added before the description of the overdue purchase order, and ending text that is added after the description of the overdue purchase order.</span></span>  

<span data-ttu-id="be567-144">Im folgenden Verfahren wird beschrieben, wie Sie den Vortext einrichten. Diese Schritte gelten jedoch auch für das Einrichten von Nachtexten.</span><span class="sxs-lookup"><span data-stu-id="be567-144">The following procedure describes how to set up beginning text messages, but the same steps apply for setting up ending text messages.</span></span>  

## <a name="to-set-up-delivery-reminder-text-messages"></a><span data-ttu-id="be567-145">Einrichten von Lieferbenachrichtigungstexten</span><span class="sxs-lookup"><span data-stu-id="be567-145">To set up delivery reminder text messages</span></span>  

1.  <span data-ttu-id="be567-146">Wählen Sie im Fenster **Lieferbenachrichtigungsstufen** eine Stufe aus, und wählen Sie dann die Aktion **Vortext**.</span><span class="sxs-lookup"><span data-stu-id="be567-146">In the **Delivery Reminder Levels** window, select a level, and then choose the **Beginning Text** action.</span></span>  
2.  <span data-ttu-id="be567-147">Wählen Sie die Aktion **Neu**.</span><span class="sxs-lookup"><span data-stu-id="be567-147">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="be567-148">Geben Sie im Feld **Beschreibung** den Vortext für die Lieferbenachrichtigung ein.</span><span class="sxs-lookup"><span data-stu-id="be567-148">In the **Description** field, enter the beginning text message for the delivery reminder.</span></span>  
4.  <span data-ttu-id="be567-149">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="be567-149">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="be567-150">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="be567-150">See Also</span></span>  
 <span data-ttu-id="be567-151">[Lieferanmahnungen](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="be567-151">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="be567-152">[Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="be567-152">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="be567-153">[So werden Lieferbenachrichtigungscodes zu Kreditoren zugewiesen](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="be567-153">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="be567-154">[So erstellen Sie Lieferanmahnungen manuell](how-to-create-delivery-reminders-manually.md) </span><span class="sxs-lookup"><span data-stu-id="be567-154">[Create Delivery Reminders Manually](how-to-create-delivery-reminders-manually.md) </span></span>  
 [<span data-ttu-id="be567-155">Lieferbenachrichtigung registrieren</span><span class="sxs-lookup"><span data-stu-id="be567-155">Issue Delivery Reminders</span></span>](how-to-issue-delivery-reminders.md)
