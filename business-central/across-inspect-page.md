---
title: Überprüfen von Seiten in Business Central
description: Verwenden Sie die Seitenüberprüfungsfunktion, um Details zum Seitenentwurf und zur Datenquelle anzuzeigen. Der Seiteninspektor eignet sich ideal zum Beheben von Problemen mit Ihren Daten.
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
author: jswymer
ms.date: 04/01/2019
ms.openlocfilehash: e747757ec6942ede0e237e013703ebf6d3df189b
ms.sourcegitcommit: dac212009aadf3227e54c99976c438f6e56f182a
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 05/02/2019
ms.locfileid: "1447031"
---
# <a name="inspecting-pages-in-business-central"></a><span data-ttu-id="cec20-104">Überprüfen von Seiten in Business Central</span><span class="sxs-lookup"><span data-stu-id="cec20-104">Inspecting Pages in Business Central</span></span>

<span data-ttu-id="cec20-105">Die Überprüfungsfunktion der Seite ermöglicht es Ihnen, Details zu einer Seite abzurufen und bietet Einblick in den Seitenentwurf, die verschiedenen Elemente, aus denen die Seite besteht und die Quelle hinter den angezeigten Daten.</span><span class="sxs-lookup"><span data-stu-id="cec20-105">The page inspection feature enables you to get details about a page, providing insight into the page design, the different elements that comprise the page, and the source behind the data it displays.</span></span> <span data-ttu-id="cec20-106">Seitenüberprüfung ist besonders für Administratoren und Superuser, Support-Mitarbeiter und Entwickler gedacht.</span><span class="sxs-lookup"><span data-stu-id="cec20-106">Page inspection is especially designed for administrators, power users, support personnel, and developers.</span></span> <span data-ttu-id="cec20-107">Es eignet sich ideal, um mehr über das Datenmodells hinter einer Seite zu erfahren, und für die Fehlerbehebung.</span><span class="sxs-lookup"><span data-stu-id="cec20-107">It is ideal for learning the data model behind a page and troubleshooting.</span></span> <span data-ttu-id="cec20-108">Wenn Sie beispielsweise ein Problem mit einer Seite haben, können Sie mit der Seitenüberprüfung Informationen erhalten, die Sie an den Systemadministrator oder den Supportmitarbeiter weitergeben.</span><span class="sxs-lookup"><span data-stu-id="cec20-108">For example, if you are experiencing a problem with a page, you could use page inspection to get information to pass on to your system administrator or support personnel.</span></span>

## <a name="working-with-page-inspection"></a><span data-ttu-id="cec20-109">Arbeiten mit der Seitenüberprüfung</span><span class="sxs-lookup"><span data-stu-id="cec20-109">Working with Page Inspection</span></span>

<span data-ttu-id="cec20-110">Starten Sie die Seitenüberprüfung über die Seite **Hilfe und Support**.</span><span class="sxs-lookup"><span data-stu-id="cec20-110">You start page inspection from the **Help & Support** page.</span></span> <span data-ttu-id="cec20-111">Wählen Sie ein Fragezeichen in der oberen rechten Ecke aus, wählen Sie **Hilfe und Support** und dann **Seiten und Daten prüfen** aus.</span><span class="sxs-lookup"><span data-stu-id="cec20-111">Choose the question mark in the top right corner, choose **Help & Support**, and then choose **Inspect pages and data**.</span></span> <span data-ttu-id="cec20-112">Zudem besteht die Möglichkeit, die Tastenkombination **Strg+Alt+F1** zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="cec20-112">Or, you can just use the keyboard shortcut **Ctrl+Alt+F1**.</span></span>

<span data-ttu-id="cec20-113">Der Bereich **Seitenüberprüfung** wird auf der Seite geöffnet.</span><span class="sxs-lookup"><span data-stu-id="cec20-113">The **Page inspection** pane opens on the side.</span></span> <span data-ttu-id="cec20-114">Die folgende Abbildung zeigt den Bereich **Seitenüberprüfung** auf der Seite **Verkaufsauftrag**.</span><span class="sxs-lookup"><span data-stu-id="cec20-114">The following figure illustrates the **Page Inspection** pane on the **Sales Order** page.</span></span>

![Seitenüberprüfung](media/page-inspection-example.png)

<span data-ttu-id="cec20-116">Wenn der Bereich **Seitenüberprüfung** erstmaligen geöffnet wird, werden Informationen zum Hauptseitenobjekt angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cec20-116">When the **Page Inspection** pane first opens, it shows information that pertains to the main page object.</span></span>

<span data-ttu-id="cec20-117">Verwenden Sie die Tastatur oder ein Zeigegerät, um den Fokus auf verschiedene Elemente der Seite zu verschieben.</span><span class="sxs-lookup"><span data-stu-id="cec20-117">Use the keyboard or pointing device to move focus to different elements on the page.</span></span> <span data-ttu-id="cec20-118">Wenn Sie eine Infobox oder einen Teil der Hauptseite auswählen, wird der umgebende Bereich von einen Rahmen markiert und der Bereich **Seitenüberprüfung** zeigt Informationen zum ausgewählten Element.</span><span class="sxs-lookup"><span data-stu-id="cec20-118">When you select a FactBox or a part on the main page, the bounding area is highlighted by a border, and the **Page Inspection** pane shows information about the selected element.</span></span> <span data-ttu-id="cec20-119">Beispielsweise zeigt die vorherige Abbildung Informationen über den Listenanteil auf der Seite **Verkaufsauftrag** an.</span><span class="sxs-lookup"><span data-stu-id="cec20-119">For example, the previous figure shows information about the list part in the **Sales Order** page.</span></span> <span data-ttu-id="cec20-120">Wenn Sie zu anderen Seiten in der Anwendung navigieren, wird der Bereich **Seitenüberprüfung** dabei automatisch mit Seiteninformationen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cec20-120">As you navigate to other pages in the application, the **Page Inspection** pane will automatically update with page information as you move along.</span></span>

<span data-ttu-id="cec20-121">Weitere Informationen darüber, was in der Seitenüberprüfung angezeigt wird, finden Sie in [Überprüfung und Fehlerbehebung von Seiten](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-inspecting-pages) in der Hilfe für Business Central-Entwickler und IT-Profis.</span><span class="sxs-lookup"><span data-stu-id="cec20-121">For more information about what is shown in page inspection, see [Inspecting and Troubleshooting Pages](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-inspecting-pages) in the Business Central Developer and IT Pro help.</span></span>

<span data-ttu-id="cec20-122">Wenn die erwarteten Details im Bereich **Seitenüberprüfung** nicht angezeigt werden, verfügen Sie möglicherweise nicht über die erforderlichen Berechtigungen, wie im nächsten Abschnitt erläutert.</span><span class="sxs-lookup"><span data-stu-id="cec20-122">If you do not see the details that you expect to see in the **Page Inspection** pane, you probably do not have the required permissions, as described in the next section.</span></span>

## <a name="controlling-access-to-page-inspection-details"></a><span data-ttu-id="cec20-123">Steuern des Zugriffs auf Seitenüberprüfungsdetails</span><span class="sxs-lookup"><span data-stu-id="cec20-123">Controlling Access to Page Inspection Details</span></span>

<span data-ttu-id="cec20-124">Als ein Administrator können Sie den Zugriff auf die gesamten Details steuern, die im Bereich **Seitenüberprüfung** angezeigt werden, indem Sie die Berechtigungen konfigurieren, die Benutzer haben.</span><span class="sxs-lookup"><span data-stu-id="cec20-124">As an administrator, you can control access to the full details that are shown in the **Page Inspection** pane by configuring the permissions that users have.</span></span> <span data-ttu-id="cec20-125">Um einem Benutzer Berechtigung für alle Details zu gewähren, geben Sie Benutzern die Berechtigung **Ausführen** im **System**-Objekt **5330**.</span><span class="sxs-lookup"><span data-stu-id="cec20-125">To grant a user permission to the full details, give users **Execute** permission on the **System** object **5330**.</span></span> <span data-ttu-id="cec20-126">Sie können diese Berechtigungen gewähren, indem Sie einen Berechtigungssatz (beispielsweise **D365 Troubleshoot**) oder eine Benutzergruppe (beispielsweise **D365 Troubleshoot**) verwenden.</span><span class="sxs-lookup"><span data-stu-id="cec20-126">You can grant this permission by using a permission set (such as **D365 Troubleshoot**) or a user group (such as **D365 Troubleshoot**).</span></span> <span data-ttu-id="cec20-127">Weitere Informationen zu Berechtigungen finden Sie unter [Verwalten von Benutzern und Berechtigungen](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="cec20-127">For more information about permissions, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>

<span data-ttu-id="cec20-128">Benutzer, die keine Berechtigungen in **Systemobjekt 5330** haben, können dennoch auf den Bereich **Seitenüberprüfung** zugreifen, sehen allerdings nur die Felder **Seite** und **Tabelle**, die grundlegende Details anzeigen, die sie an ihr Support Team weitergeben können.</span><span class="sxs-lookup"><span data-stu-id="cec20-128">Users who are not granted permissions on **System object 5330** can still access the **Page Inspection** pane, but they will only see the **Page** and **Table** fields, which display basic details that they can pass on to their support team.</span></span>

## <a name="see-also"></a><span data-ttu-id="cec20-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cec20-129">See Also</span></span>

<span data-ttu-id="cec20-130">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cec20-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  