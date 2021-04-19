---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5609b99f8d05402b79c22fee8f7a70dc7e82b22c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771536"
---
<span data-ttu-id="f9d98-101">Lieferbenachrichtigungen dienen dazu, überfällige Kreditorlieferungen zu verfolgen und Kreditoren an überfällige Lieferungen zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="f9d98-101">Delivery reminders are used to track overdue vendor shipments and to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="f9d98-102">Zur Erstellung von Lieferbenachrichtigungen müssen Sie Folgendes einrichten:</span><span class="sxs-lookup"><span data-stu-id="f9d98-102">To create delivery reminders, you must set up the following:</span></span>

- <span data-ttu-id="f9d98-103">Lieferbenachrichtigungsmethoden</span><span class="sxs-lookup"><span data-stu-id="f9d98-103">Delivery reminder terms</span></span>  

    <span data-ttu-id="f9d98-104">Lieferbenachrichtigungsmethoden werden durch einen Code identifiziert, der Kreditoren zugewiesen werden muss.</span><span class="sxs-lookup"><span data-stu-id="f9d98-104">Delivery reminder terms are identified by a code that must be assigned to vendors.</span></span> <span data-ttu-id="f9d98-105">Um mehrere Einstellungskombinationen verwenden zu können, müssen Sie jeweils für jede Einstellung getrennt einen Code festlegen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-105">To use more than one combination of settings, you must set up a code for each setting separately.</span></span> <span data-ttu-id="f9d98-106">Sie können eine beliebige Anzahl an Lieferbenachrichtigungsmethoden einrichten.</span><span class="sxs-lookup"><span data-stu-id="f9d98-106">You can set up any number of delivery reminder terms.</span></span>  

- <span data-ttu-id="f9d98-107">Lieferbenachrichtigungsstufen</span><span class="sxs-lookup"><span data-stu-id="f9d98-107">Delivery reminder levels</span></span>  

    <span data-ttu-id="f9d98-108">Für jede Lieferbenachrichtigungsmethode müssen gesonderte Lieferbenachrichtigungstexte festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="f9d98-108">For every delivery reminder term, you must set up delivery reminder levels.</span></span> <span data-ttu-id="f9d98-109">Diese Stufen bestimmen, wie oft Lieferbenachrichtigungen für eine bestimmte Methode erzeugt werden können.</span><span class="sxs-lookup"><span data-stu-id="f9d98-109">These levels determine how often delivery reminders can be created for a specific term.</span></span> <span data-ttu-id="f9d98-110">Stufe 1 ist die erste Lieferbenachrichtigung, die Sie für eine überfällige Lieferung erstellen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-110">Level 1 is the first delivery reminder that you create for an overdue delivery.</span></span> <span data-ttu-id="f9d98-111">Stufe 2 ist die zweite Lieferbenachrichtigung und so weiter.</span><span class="sxs-lookup"><span data-stu-id="f9d98-111">Level 2 is the second delivery reminder, and so on.</span></span> <span data-ttu-id="f9d98-112">Bei der Erstellung von Lieferbenachrichtigungen wird die Anzahl der zuvor erstellten Benachrichtigungen berücksichtigt und die für die aktuelle Anzahl definierte Methode verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9d98-112">When delivery reminders are created, the number of reminders that were created previously is considered, and the current number is used to apply terms.</span></span>  

- <span data-ttu-id="f9d98-113">Lieferbenachrichtigungstexte</span><span class="sxs-lookup"><span data-stu-id="f9d98-113">Delivery reminder texts messages</span></span>  

    <span data-ttu-id="f9d98-114">Sie müssen für jede Lieferbenachrichtigungsstufe gesonderte Lieferbenachrichtigungstexte festlegen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-114">You must set up delivery reminder text messages for every delivery reminder level.</span></span> <span data-ttu-id="f9d98-115">Es gibt zwei Arten von Lieferbenachrichtigungstexten: Vortexte und Nachtexte.</span><span class="sxs-lookup"><span data-stu-id="f9d98-115">There are two types of delivery reminder text messages: beginning and ending.</span></span> <span data-ttu-id="f9d98-116">Der Vortext wird unter dem Kopf vor der Liste von Einträgen, die angemahnt werden, gedruckt.</span><span class="sxs-lookup"><span data-stu-id="f9d98-116">The beginning text message is printed under the header section, before the list of entries that are marked for reminder.</span></span> <span data-ttu-id="f9d98-117">Der Nachtext wird nach dieser Liste gedruckt.</span><span class="sxs-lookup"><span data-stu-id="f9d98-117">The ending text message is printed after this list.</span></span>  

<span data-ttu-id="f9d98-118">Nach dem Einrichten der Lieferbestimmungen, -stufen und -texte müssen Sie den Kreditoren die entsprechenden Lieferanmahnungscodes zuweisen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-118">After you have set up the delivery terms, levels, and texts, you must assign the relevant delivery reminder codes to your vendors.</span></span>  

<span data-ttu-id="f9d98-119">Lieferbenachrichtigungen können manuell oder automatisch erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f9d98-119">You can create delivery reminders manually or automatically.</span></span> <span data-ttu-id="f9d98-120">Sie können den Batchauftrag **Lieferanmahnung erstellen** zum automatischen Erstellen von Lieferanmahnungen nutzen, damit Sie die Bestellungen auswählen können, für die Lieferanmahnungen erstellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-120">You can use the **Create Delivery Reminder** batch job to create delivery reminders automatically so that you can select the purchase orders for which delivery reminders must be created.</span></span>  

<span data-ttu-id="f9d98-121">Sie können Dokumente auch in Bezug auf Bestell- oder Auftragspositionen verfolgen.</span><span class="sxs-lookup"><span data-stu-id="f9d98-121">You can also track documents in relation to purchase order lines and sales order lines.</span></span>  

[!INCLUDE[prod_short](../../../includes/prod_short.md)] <span data-ttu-id="f9d98-122">stellt die folgenden Berichte bereit:</span><span class="sxs-lookup"><span data-stu-id="f9d98-122">provides the following reports:</span></span>  

- <span data-ttu-id="f9d98-123">**Reg. Lieferbenachrichtigung** – Zum Anzeigen der Lieferbenachrichtigungen für Kreditoren.</span><span class="sxs-lookup"><span data-stu-id="f9d98-123">**Issued Delivery Reminder** - To view the delivery reminders for vendors.</span></span>  
- <span data-ttu-id="f9d98-124">**Lieferbenachrichtigung - Test** - Zum Überprüfen der Lieferbenachrichtigungen vor deren Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="f9d98-124">**Delivery Reminder - Test** - To verify the delivery reminders before you issue them.</span></span>  
