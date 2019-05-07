---
title: "So geht's: Kostenbudgetposten löschen | Microsoft Docs"
description: Sie verwenden den Batchauftrag Kostenbudgeteinträge löschen , um Kostenbudgetposten in der Kostenbudgeterfassung zu stornieren.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 5271085256c9611941b5378231d603174328dc39
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 03/31/2019
ms.locfileid: "921888"
---
# <a name="delete-cost-budget-entries"></a><span data-ttu-id="dd320-103">Kostenbudgetposten löschen</span><span class="sxs-lookup"><span data-stu-id="dd320-103">Delete Cost Budget Entries</span></span>
<span data-ttu-id="dd320-104">Sie verwenden den Batchauftrag **Kostenbudgeteinträge löschen** , um Kostenbudgetposten in der Kostenbudgeterfassung zu stornieren.</span><span class="sxs-lookup"><span data-stu-id="dd320-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="dd320-105">Um keine Lücken in den Kostenbudgetposten und den Kostenjournalposten entstehen zu lassen, können Sie einen einzelnen Posten oder eine Gruppe von Posten nicht mitten in der Liste der Journalposten löschen.</span><span class="sxs-lookup"><span data-stu-id="dd320-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="dd320-106">Kostenbudgetposten löschen:</span><span class="sxs-lookup"><span data-stu-id="dd320-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="dd320-107">Wählen Sie das Symbol ![Glühlampe, mit der die Funktion „Wie möchten Sie weiter verfahren“ geöffnet wird](media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") aus, geben Sie **Budgeteinträge löschen** ein, und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="dd320-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="dd320-108">Die **Zu-Register-Nr.**</span><span class="sxs-lookup"><span data-stu-id="dd320-108">The **To Register No.**</span></span> <span data-ttu-id="dd320-109">Das Feld  enthält die letzte Journalpostennummer und kann nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="dd320-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="dd320-110">Sie können **Von Journalnr.** verwenden</span><span class="sxs-lookup"><span data-stu-id="dd320-110">You can use the **From Register No.**</span></span> <span data-ttu-id="dd320-111">Sie können das Feld  verwenden, um eine Journalpostennummer auszuwählen, ab der der Löschvorgang beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="dd320-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="dd320-112">Wählen Sie die Schaltfläche **OK** aus, um die ausgewählten Kostenbudgetposten zu löschen.</span><span class="sxs-lookup"><span data-stu-id="dd320-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="dd320-113">Um ein versehentliches Löschen von Kostenbudgetposten zu vermeiden, können Sie Journalposten schließen, indem Sie die Zeilen als **Abgeschlossen** im Feld **Abgeschlossen** auf der Seite **Kostenbudget-Register**markieren.</span><span class="sxs-lookup"><span data-stu-id="dd320-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field on the **Cost Budget Registers** page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="dd320-114">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="dd320-114">See Also</span></span>  
<span data-ttu-id="dd320-115">[Kostenrechnung](finance-manage-cost-accounting.md)
[Erstellen von Kostenbudgets](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="dd320-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="dd320-116">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dd320-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
