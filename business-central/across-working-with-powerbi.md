---
title: Arbeiten mit Power BI-Berichten in Business Central | Microsoft Docs
description: Insight, Business Intelligence und KPIs aus Ihren Business Central Daten einfach beziehen mit der Business Central Anwendung für Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 28e332137346aae320b73c326bb3a41d3b7e7097
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927214"
---
# <a name="working-with-power-bi-reports-in-prodshort"></a><span data-ttu-id="1e224-103">Arbeiten mit Power BI-Berichten in [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="1e224-103">Working with Power BI Reports in [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

<span data-ttu-id="1e224-104">In diesem Artikel erlernen Sie einige der Grundlagen zum Anzeigen von Power BI-Berichten in [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="1e224-104">In this article, you learn some of the basics about viewing Power BI reports in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

## <a name="overview"></a><span data-ttu-id="1e224-105">Matrix</span><span class="sxs-lookup"><span data-stu-id="1e224-105">Overview</span></span>

<span data-ttu-id="1e224-106">Power BI-Berichte geben Ihnen Einblick in Ihre [!INCLUDE[prodshort](includes/prodshort.md)]-Daten.</span><span class="sxs-lookup"><span data-stu-id="1e224-106">Power BI reports give you insight into your [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="1e224-107">Verschiedene Seiten in [!INCLUDE [prodshort](includes/prodshort.md)] umfassen einen Power BI-Berichtsteil, in dem Power BI-Berichte angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="1e224-107">Various pages in [!INCLUDE [prodshort](includes/prodshort.md)] include a Power BI reports part that can display Power BI reports.</span></span> <span data-ttu-id="1e224-108">Das Rollencenter ist eine typische Seite, auf der Sie einen Power BI-Berichtsteil anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="1e224-108">The role center is a typical page where you'll see a Power BI reports part.</span></span> <span data-ttu-id="1e224-109">Einige Listenseiten, wie z. B. **Artikel** , umfassen außerdem einen Power BI-Teil.</span><span class="sxs-lookup"><span data-stu-id="1e224-109">Some list pages, like **Items** , also include a Power BI part.</span></span>

<span data-ttu-id="1e224-110">[!INCLUDE [prodshort](includes/prodshort.md)] arbeitet mit dem Power BI-Dienst zusammen.</span><span class="sxs-lookup"><span data-stu-id="1e224-110">[!INCLUDE [prodshort](includes/prodshort.md)] works together with the Power BI service.</span></span> <span data-ttu-id="1e224-111">Berichte zur Anzeige in [!INCLUDE [prodshort](includes/prodshort.md)] werden in einem Power BI-Dienst gespeichert.</span><span class="sxs-lookup"><span data-stu-id="1e224-111">Reports for displaying in [!INCLUDE [prodshort](includes/prodshort.md)] are stored in a Power BI service.</span></span> <span data-ttu-id="1e224-112">In [!INCLUDE [prodshort](includes/prodshort.md)] können Sie im Power BI-Teil jeden Power BI-Bericht anzeigen, der in Ihrem Power BI-Dienst verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="1e224-112">In [!INCLUDE [prodshort](includes/prodshort.md)], you can switch the report displayed in the Power BI part to any Power BI report available in your Power BI service.</span></span> <span data-ttu-id="1e224-113">Wenn Sie sich zum ersten Mal bei [!INCLUDE [prodshort](includes/prodshort.md)] anmelden und bis zum Herstellen einer Verbindung zu einem Power BI-Dienst sind die Teile leer, wie hier zu sehen ist:</span><span class="sxs-lookup"><span data-stu-id="1e224-113">The first time you sign into [!INCLUDE [prodshort](includes/prodshort.md)], and until you connect to a Power BI service, parts will be empty, as shown here:</span></span>

![Power BI-Teil in Business Central](./media/power-bi-part.png)

## <a name="prerequisites"></a><span data-ttu-id="1e224-115">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e224-115">Prerequisites</span></span>

<span data-ttu-id="1e224-116">Wenn Sie [!INCLUDE[prodshort](includes/prodshort.md)] on-premises verwenden, muss es für die Power BI-Integration aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="1e224-116">If you're using [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, it must be enabled for Power BI integration.</span></span> <span data-ttu-id="1e224-117">Diese Aufgabe wird normalerweise von einem Administrator ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1e224-117">This task is typically done by an administrator.</span></span> <span data-ttu-id="1e224-118">Weitere Informationen finden Sie unter [[!INCLUDE[prodshort](includes/prodshort.md)] on-premises für die Power BI-Integration einrichten](admin-powerbi-setup.md#setup).</span><span class="sxs-lookup"><span data-stu-id="1e224-118">For more information, see [Set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for Power BI integration](admin-powerbi-setup.md#setup).</span></span>

> [!NOTE]
> [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="1e224-119">online ist bereits für die Integration von Power BI eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="1e224-119">online is already set up to integrate with Power BI.</span></span>

## <a name="get-ready"></a><span data-ttu-id="1e224-120">Vorbereitung</span><span class="sxs-lookup"><span data-stu-id="1e224-120">Get ready</span></span>

<span data-ttu-id="1e224-121">Registrieren Sie sich für den Power BI-Dienst.</span><span class="sxs-lookup"><span data-stu-id="1e224-121">Sign up for the Power BI service.</span></span> <span data-ttu-id="1e224-122">Wenn Sie sich noch nicht registriert haben, wechseln Sie zu [https://powerbi.microsoft.com](https://powerbi.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1e224-122">If you haven't already signed up, go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com).</span></span> <span data-ttu-id="1e224-123">Verwenden Sie bei der Registrierung Ihre geschäftliche E-Mail-Adresse und Ihr Kennwort.</span><span class="sxs-lookup"><span data-stu-id="1e224-123">When you sign up, use your work email address and password.</span></span>

## <a name="connect-to-power-bi---one-time-only"></a><span data-ttu-id="1e224-124">Mit Power BI verbinden – nur ein Mal</span><span class="sxs-lookup"><span data-stu-id="1e224-124">Connect to Power BI - one time only</span></span>

<span data-ttu-id="1e224-125">Wenn Sie sich zum ersten Mal bei [!INCLUDE [prodshort](includes/prodshort.md)] anmelden, sehen Sie auf einigen Seiten eventuell einen leeren Power BI-Teil, wie in der vorherigen Abbildung gezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-125">When you first sign into [!INCLUDE [prodshort](includes/prodshort.md)], you might see an empty Power BI part on some page, as shown in the previous figure.</span></span> <span data-ttu-id="1e224-126">In diesem Fall müssen Sie sich zuerst mit Ihrem Power BI-Konto verbinden.</span><span class="sxs-lookup"><span data-stu-id="1e224-126">The first thing to do is to connect to your Power BI account.</span></span> <span data-ttu-id="1e224-127">Sobald die Verbindung hergestellt ist, werden Berichte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-127">Once connected, you can see reports.</span></span> <span data-ttu-id="1e224-128">Sie müssen diesen Schritt nur einmal ausführen.</span><span class="sxs-lookup"><span data-stu-id="1e224-128">You only have to do this step once.</span></span>

<span data-ttu-id="1e224-129">Um eine Verbindung zu Power BI herzustellen, wählen Sie die Verknüpfung **Erste Schritte mit Power BI** im Teil **Power BI-Berichte** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-129">To connect to Power BI, select the **Get Started with Power BI** link in the **Power BI Reports** part.</span></span>

<span data-ttu-id="1e224-130">Während des Verbindungsvorgangs kommuniziert [!INCLUDE [prodshort](includes/prodshort.md)] mit dem Power BI-Dienst, um festzustellen, ob Sie über ein gültiges Konto und eine gültige Lizenz für Power BI verfügen.</span><span class="sxs-lookup"><span data-stu-id="1e224-130">During the connecting process, [!INCLUDE [prodshort](includes/prodshort.md)] communicates with the Power BI service to determine if you have a valid Power BI account and license.</span></span> <span data-ttu-id="1e224-131">Sobald Ihre Lizenz überprüft wurde, wird der Power BI-Standardbericht auf der Seite angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-131">Once your license is verified, the default Power BI report displays on the page.</span></span> <span data-ttu-id="1e224-132">Wenn dort kein Bericht angezeigt wird, können Sie einen Bericht aus dem Teil auswählen.</span><span class="sxs-lookup"><span data-stu-id="1e224-132">If there a report isn't shown, you can select a report from the part.</span></span>

> [!TIP]
> <span data-ttu-id="1e224-133">Mit [!INCLUDE [prodshort](includes/prodshort.md)] online werden in diesem Schritt automatisch die Power BI-Standardberichte, die in [!INCLUDE [prodshort](includes/prodshort.md)] verwendet werden, in Ihren Power BI-Arbeitsbereich hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="1e224-133">With [!INCLUDE [prodshort](includes/prodshort.md)] online, this this step will automatically upload default Power BI reports used in [!INCLUDE [prodshort](includes/prodshort.md)] to your Power BI workspace.</span></span>

##### <a name="from-prodshort-on-premises"></a><span data-ttu-id="1e224-134">Aus [!INCLUDE [prodshort](includes/prodshort.md)] on-premises</span><span class="sxs-lookup"><span data-stu-id="1e224-134">From [!INCLUDE [prodshort](includes/prodshort.md)] on-premises</span></span>

<span data-ttu-id="1e224-135">Das Verbinden mit Power BI erfolgt auf ähnliche Weise wie bei [!INCLUDE [prodshort](includes/prodshort.md)] online.</span><span class="sxs-lookup"><span data-stu-id="1e224-135">Connecting to Power BI from [!INCLUDE [prodshort](includes/prodshort.md)] is similar to online.</span></span> <span data-ttu-id="1e224-136">Auf der Seite **AZURE ACTIVE DIRECTORY-DIENSTBERECHTIGUNGEN** werden Sie jedoch aufgefordert, Zugriff auf die Power BI-Dienste zu gewähren.</span><span class="sxs-lookup"><span data-stu-id="1e224-136">However, you'll be prompted on the **AZURE ACTIVE DIRECTORY SERVICE PERMISSIONS** page to grant access to Power BI Services.</span></span> <span data-ttu-id="1e224-137">Um den Zugriff zu gewähren, wählen Sie **Azure Services genehmigen** und dann **Akzeptieren** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-137">To grant access, select **Authorize Azure Services** , and then **Accept** .</span></span>

<span data-ttu-id="1e224-138">Sobald die Verbindung hergestellt ist, können Sie auf den Seiten einen Bericht aus dem Power BI-Teil auswählen.</span><span class="sxs-lookup"><span data-stu-id="1e224-138">Once connected, you can select a report from the Power BI part on pages.</span></span>

## <a name="show-power-bi-reports-on-list-pages"></a><span data-ttu-id="1e224-139">Power BI-Berichte auf Listenseiten anzeigen</span><span class="sxs-lookup"><span data-stu-id="1e224-139">Show Power BI reports on list pages</span></span>

[!INCLUDE[prodlong](includes/prodlong.md)] <span data-ttu-id="1e224-140">umfasst eine Power BI-Infobox auf mehreren Schlüssellistenseiten.</span><span class="sxs-lookup"><span data-stu-id="1e224-140">includes a Power BI FactBox on several key list pages.</span></span> <span data-ttu-id="1e224-141">Diese Infobox bietet zusätzliche Einblicke in die Daten in der Liste.</span><span class="sxs-lookup"><span data-stu-id="1e224-141">This FactBox provides additional insight into the data in the list.</span></span> <span data-ttu-id="1e224-142">Während Sie sich zwischen den Zeilen in der Liste bewegen, wird der Bericht für den Eintrag gefiltert und aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="1e224-142">As you move between rows in the list, the report is updated and filtered for the selected entry.</span></span> <span data-ttu-id="1e224-143">Wenn Sie diesen Teil nicht sehen, wählen Sie in der Aktionsleiste **Aktionen** > **Anzeigen** > **Power BI-Berichte anzeigen/ausblenden** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-143">If you don't see this part, then from the action bar, select **Actions** > **Display** > **Show/Hide Power BI Reports** .</span></span> <span data-ttu-id="1e224-144">Weitere Informationen finden Sie unter [Erstellen von Power BI-Berichten zum Anzeigen von Listendaten in [!INCLUDE[prodshort](includes/prodshort.md)]](across-how-use-powerbi-reports-factbox.md).</span><span class="sxs-lookup"><span data-stu-id="1e224-144">For more information, see [Creating Power BI Reports for Displaying List Data in [!INCLUDE[prodshort](includes/prodshort.md)]](across-how-use-powerbi-reports-factbox.md).</span></span>

## <a name="select-power-bi-reports"></a><span data-ttu-id="1e224-145">Power BI-Berichte auswählen</span><span class="sxs-lookup"><span data-stu-id="1e224-145">Select Power BI reports</span></span>

<span data-ttu-id="1e224-146">Ein Power BI-Teil auf einer Seite kann jeden Power BI-Bericht anzeigen, der für Sie verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="1e224-146">A Power BI part on a page can display any Power BI report that's available to you.</span></span> <span data-ttu-id="1e224-147">Um einen anderen Bericht anzuzeigen, wählen Sie oben aus der Dropdown-Befehlsliste die Aktion **Bericht auswählen** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-147">To switch to view another report, choose the **Select Report** action from the drop-down command list at the top of the part.</span></span>  

<span data-ttu-id="1e224-148">Die Seite **Power BI-Berichtsauswahl** zeigt eine Liste aller Power BI-Berichte an, auf die Sie Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="1e224-148">The **Power BI Reports Selection** page shows a list of all the Power BI reports that you have access to.</span></span> <span data-ttu-id="1e224-149">Diese Liste wird von Ihrem Power BI Arbeitsplatz abgerufen.</span><span class="sxs-lookup"><span data-stu-id="1e224-149">This list is retrieved from your Power BI workspace.</span></span> <span data-ttu-id="1e224-150">Aktivieren Sie für jeden Bericht, den Sie auf der Startseite anzeigen möchten, das Kontrollkästchen **Aktivieren** . Wählen Sie dann **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-150">Select the **Enable** box for each report that you want to display on the page, and then choose **OK** .</span></span> <span data-ttu-id="1e224-151">Sie kehren zur Seite zurück und der zuletzt aktivierte Bericht wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-151">You'll return to the page, and the last report you enabled will appear.</span></span> <span data-ttu-id="1e224-152">Verwenden Sie die Befehle **Zurück** und **Nächster** aus der Dropdown-Befehlsliste, um zwischen Berichten zu navigieren.</span><span class="sxs-lookup"><span data-stu-id="1e224-152">Using the drop-down command list, use the **Previous** and **Next** commands to navigate between reports.</span></span>  

## <a name="get-reports"></a><span data-ttu-id="1e224-153">Berichte abrufen</span><span class="sxs-lookup"><span data-stu-id="1e224-153">Get reports</span></span>

<span data-ttu-id="1e224-154">Wenn auf der Seite **Power BI-Berichtsauswahl** kein bzw. nicht der gewünschte Bericht angezeigt wird, wählen Sie **Berichte abrufen** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-154">If you don't see any reports on the **Power BI Reports Selection** page, or don't see the report you want, choose **Get Reports** .</span></span> <span data-ttu-id="1e224-155">Mit dieser Aktion können Sie von den folgenden zwei Orten aus nach Berichten suchen: *Meine Organisation* oder *Dienste* .</span><span class="sxs-lookup"><span data-stu-id="1e224-155">This action lets you look for reports from two locations: *My Organization* or from *Services* .</span></span>

- <span data-ttu-id="1e224-156">Wählen Sie **Meine Organisation** aus, um zu den Power BI-Diensten zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="1e224-156">Choose **My Organization** to go to the Power BI services.</span></span> <span data-ttu-id="1e224-157">Von hier aus können Sie die Berichte in Ihrer Organisation anzeigen, für die Sie zur Anzeige berechtigt sind.</span><span class="sxs-lookup"><span data-stu-id="1e224-157">From here, you can view the reports within your organization that you've been given rights to view.</span></span> <span data-ttu-id="1e224-158">Diese Berichte können Sie dann Ihrem Arbeitsbereich hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1e224-158">You can then add them to your workspace.</span></span>
- <span data-ttu-id="1e224-159">Wählen **Dienstleistungen** , um zum Microsoft AppSource zu gehen, wo Sie Power BI Apps installieren können.</span><span class="sxs-lookup"><span data-stu-id="1e224-159">Choose **Services** to go to Microsoft AppSource where you can install Power BI apps.</span></span>  

> [!TIP]
> <span data-ttu-id="1e224-160">Falls Sie mit Power BI Desktop arbeiten, können Sie außerdem neue Power BI-Berichte erstellen.</span><span class="sxs-lookup"><span data-stu-id="1e224-160">If you have Power BI Desktop, you can also create new Power BI reports.</span></span> <span data-ttu-id="1e224-161">Sobald diese Berichte in Ihrem Power BI-Arbeitsbereich veröffentlicht wurden, werden sie auf der Seite **Power BI-Berichtsauswahl** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-161">Then, once those reports are published to your Power BI workspace, they will appear on the **Power BI Reports Selection** page.</span></span>  

## <a name="manage-and-modify-reports"></a><span data-ttu-id="1e224-162">Berichte verwalten und ändern</span><span class="sxs-lookup"><span data-stu-id="1e224-162">Manage and modify reports</span></span>

<span data-ttu-id="1e224-163">Im Power BI-Teil können Sie Änderungen an einem Bericht vornehmen.</span><span class="sxs-lookup"><span data-stu-id="1e224-163">You can make changes to a report in the Power BI part.</span></span> <span data-ttu-id="1e224-164">Die von Ihnen vorgenommenen Änderungen werden dann im Power BI-Dienst veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="1e224-164">The changes that you make will then be published to the Power BI service.</span></span> <span data-ttu-id="1e224-165">Wenn der Bericht mit anderen Benutzern geteilt wird, können diese die Änderungen ebenfalls sehen, sofern Sie die Änderungen nicht in einem neuen Bericht speichern.</span><span class="sxs-lookup"><span data-stu-id="1e224-165">If the report is shared with other users, they'll also see the changes, unless you save the changes to a new report.</span></span>

<span data-ttu-id="1e224-166">Um einen Bericht zu ändern, wählen Sie die Aktion **Bericht verwalten** aus der Dropdown-Befehlsliste im Power BI-Teil aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-166">To modify a report, choose the **Manage Report** action from the drop-down command list in the Power BI part.</span></span> <span data-ttu-id="1e224-167">Nehmen Sie dann die gewünschten Änderungen vor.</span><span class="sxs-lookup"><span data-stu-id="1e224-167">Then start making changes.</span></span> <span data-ttu-id="1e224-168">Wenn Sie fertig sind, wählen Sie **Datei** > **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-168">Once you finish making changes, select **File** > **Save** .</span></span> <span data-ttu-id="1e224-169">Wenn es sich um einen geteilten Bericht handelt und Sie die Änderung nicht für alle Benutzer vornehmen möchten, wählen Sie **Speichern unter** aus, damit diese Änderung nicht für alle Benutzer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="1e224-169">If it's a shared report, and you don't want to make the change for all users, select **Save As** to avoid making this change for all users.</span></span>

<span data-ttu-id="1e224-170">Wenn Sie zum Rollencenter zurückkehren, wird der aktualisierte Bericht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1e224-170">When you return to the role center, the updated report will appear.</span></span> <span data-ttu-id="1e224-171">Wenn Sie **Speichern unter** verwendet haben, müssen Sie **Bericht auswählen** auswählen und den neuen Bericht anschließend aktivieren, um ihn anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="1e224-171">If you used **Save As** , you'll have to choose **Select Report** , and then enable the new report to see it.</span></span>

> [!NOTE]
> <span data-ttu-id="1e224-172">Diese Funktion steht mit [!INCLUDE [prodshort](includes/prodshort.md)] on-premises nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="1e224-172">This capability is not available with [!INCLUDE [prodshort](includes/prodshort.md)] on-premises.</span></span>

## <a name="upload-reports"></a><a name="upload"></a><span data-ttu-id="1e224-173">Berichte hochladen</span><span class="sxs-lookup"><span data-stu-id="1e224-173">Upload reports</span></span>

<span data-ttu-id="1e224-174">Power BI-Berichte können als .pbix-Dateien unter den Benutzern verteilt werden.</span><span class="sxs-lookup"><span data-stu-id="1e224-174">Power BI Reports can be distributed among users as .pbix files.</span></span> <span data-ttu-id="1e224-175">Wenn .pbix-Dateien vorhanden sind, können Sie diese hochladen und mit allen Benutzern von [!INCLUDE [prodshort](includes/prodshort.md)] teilen.</span><span class="sxs-lookup"><span data-stu-id="1e224-175">If you have any .pbix files, you can upload and share them with all users of [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="1e224-176">Die Berichte werden in jedem Unternehmen in [!INCLUDE [prodshort](includes/prodshort.md)] geteilt.</span><span class="sxs-lookup"><span data-stu-id="1e224-176">The reports are shared within each company in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>  

<span data-ttu-id="1e224-177">Um einen vorhandenen Bericht hochzuladen, wählen Sie die Aktion **Bericht hochladen** aus der Dropdown-Befehlsliste im Teil **Power BI-Berichte** aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-177">To upload a report, select the **Upload Report** action from the drop-down command list on the **Power BI Reports** part.</span></span> <span data-ttu-id="1e224-178">Suchen Sie dann nach der .pbix-Datei, die den Bericht definiert, den Sie teilen möchten.</span><span class="sxs-lookup"><span data-stu-id="1e224-178">Then, locate the .pbix file that defines the reports that you want to share.</span></span> <span data-ttu-id="1e224-179">Sie können den Standardnamen der Datei ändern.</span><span class="sxs-lookup"><span data-stu-id="1e224-179">You can change the default name of the file.</span></span>  

<span data-ttu-id="1e224-180">Nachdem der Bericht in Ihren Power BI-Arbeitsbereich hochgeladen wurde, wird er automatisch in die Power BI-Arbeitsbereiche anderer Benutzer hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="1e224-180">After the report uploads to your Power BI workspace, it automatically uploads to other users' Power BI workspaces.</span></span>

> [!NOTE]
> <span data-ttu-id="1e224-181">Zum Hochladen eines Berichts benötigen Sie SUPERUSER-Berechtigungen in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="1e224-181">Uploading a report requires that you have SUPER user permissions in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="1e224-182">Außerdem ist das Hochladen von Berichten mit [!INCLUDE [prodshort](includes/prodshort.md)] on-premises nicht möglich.</span><span class="sxs-lookup"><span data-stu-id="1e224-182">Also, you can't upload reports with [!INCLUDE [prodshort](includes/prodshort.md)] on-premises.</span></span> <span data-ttu-id="1e224-183">Mit der lokalen Version laden Sie Berichte direkt in Ihren Power BI-Arbeitsbereich hoch.</span><span class="sxs-lookup"><span data-stu-id="1e224-183">With on-premises, you upload reports directly to your Power BI workspace.</span></span> <span data-ttu-id="1e224-184">Weitere Informationen finden Sie unter [Arbeiten mit [!INCLUDE [prodshort](includes/prodshort.md)]-Daten in Power BI](across-working-with-business-central-in-powerbi.md).</span><span class="sxs-lookup"><span data-stu-id="1e224-184">For more information, see [Working with [!INCLUDE [prodshort](includes/prodshort.md)] Data In Power BI](across-working-with-business-central-in-powerbi.md).</span></span>

## <a name="fixing-problems"></a><span data-ttu-id="1e224-185">Probleme beheben</span><span class="sxs-lookup"><span data-stu-id="1e224-185">Fixing problems</span></span>

<span data-ttu-id="1e224-186">Wenn etwas schief geht, stellt dieser Abschnitt eine Problemumgehung für die häufigsten Probleme bereit.</span><span class="sxs-lookup"><span data-stu-id="1e224-186">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>  

### <a name="you-dont-have-a-power-bi-account"></a><span data-ttu-id="1e224-187">Kein Power BI-Konto vorhanden</span><span class="sxs-lookup"><span data-stu-id="1e224-187">You don't have a Power BI account</span></span>

<span data-ttu-id="1e224-188">Es wurde kein Power BI-Konto eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="1e224-188">A Power BI account hasn't been set up.</span></span> <span data-ttu-id="1e224-189">Für ein gültiges Power BI-Konto benötigen Sie eine Lizenz und müssen sich zuvor bei Power BI angemeldet haben, um einen Power BI-Arbeitsbereich zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1e224-189">To get a valid Power BI account, you must have a license, and you must have previously signed into Power BI to create a Power BI workspace.</span></span>   

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a><span data-ttu-id="1e224-190">Nachricht: Es sind keine Berichte aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1e224-190">Message: There are no enabled reports.</span></span> <span data-ttu-id="1e224-191">Wählen Sie „Bericht auswählen“ aus, um eine Liste der anzeigbaren Berichte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="1e224-191">Choose Select Report to see a list of reports that you can display.</span></span>

<span data-ttu-id="1e224-192">Diese Meldung wird angezeigt, wenn der Standardbericht nicht in Ihrem Power BI-Arbeitsbereich bereitgestellt werden konnte.</span><span class="sxs-lookup"><span data-stu-id="1e224-192">This message appears if the default report failed to deploy to your Power BI workspace.</span></span> <span data-ttu-id="1e224-193">Oder er wurde bereitgestellt, aber nicht erfolgreich aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="1e224-193">Or it deployed but didn't refresh successfully.</span></span> <span data-ttu-id="1e224-194">Navigieren Sie zum Bericht in Ihrem Power BI-Arbeitsbereich, wählen Sie **Datensatz** , **Einstellungen** aus und aktualisieren Sie die Anmeldedaten manuell.</span><span class="sxs-lookup"><span data-stu-id="1e224-194">Navigate to the report in your Power BI workspace, select **Dataset** , **Settings** , and then manually update the credentials.</span></span> <span data-ttu-id="1e224-195">Wenn der Datensatz erfolgreich aktualisiert wurde, navigieren Sie zurück zu [!INCLUDE[prodshort](includes/prodshort.md)] und wählen Sie den Bericht auf der Seite **Berichte auswählen** manuell aus.</span><span class="sxs-lookup"><span data-stu-id="1e224-195">Once the dataset successfully refreshes, navigate back to [!INCLUDE[prodshort](includes/prodshort.md)] and manually select the report from the **Select Reports** page.</span></span>


## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="1e224-196">Das dazugehörige Training finden Sie unter [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="1e224-196">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="1e224-197">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1e224-197">See Also</span></span>

[<span data-ttu-id="1e224-198">Business Central und Power BI</span><span class="sxs-lookup"><span data-stu-id="1e224-198">Business Central and Power BI</span></span>](admin-powerbi.md)  
<span data-ttu-id="1e224-199">[Power BI-Berichte erstellenl zur Anzeige von [!INCLUDE [prodlong](includes/prodlong.md)]-Daten](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-199">[Building Power BI Reports to Display [!INCLUDE [prodlong](includes/prodlong.md)] Data](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="1e224-200">[Übersicht über die Power BI-Integrationskomponente und -Architektur für [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-200">[Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)</span></span>  
<span data-ttu-id="1e224-201">[Arbeiten mit [!INCLUDE [prodshort](includes/prodshort.md)]-Daten in Power BI](across-working-with-business-central-in-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-201">[Working with [!INCLUDE [prodshort](includes/prodshort.md)] Data in Power BI](across-working-with-business-central-in-powerbi.md)</span></span>  
[<span data-ttu-id="1e224-202">Power BI für Verbraucher</span><span class="sxs-lookup"><span data-stu-id="1e224-202">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="1e224-203">Der "neue Look" des Power BI Service</span><span class="sxs-lookup"><span data-stu-id="1e224-203">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="1e224-204">Schnellstart: Stellen Sie eine Verbindung zu Daten her in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="1e224-204">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="1e224-205">Power BI Dokumentation</span><span class="sxs-lookup"><span data-stu-id="1e224-205">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="1e224-206">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="1e224-206">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="1e224-207">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="1e224-207">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="1e224-208">Geschäftsdaten aus anderen Finanzsystemen importieren</span><span class="sxs-lookup"><span data-stu-id="1e224-208">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="1e224-209">[Einrichten [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-209">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
<span data-ttu-id="1e224-210">[Verwenden von [!INCLUDE[d365fin](includes/d365fin_md.md)] als Power BI-Datenquelle](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-210">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="1e224-211">[Verwenden von [!INCLUDE[d365fin](includes/d365fin_md.md)] als Power Apps-Datenquelle](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-211">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="1e224-212">[Verwenden von [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="1e224-212">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  