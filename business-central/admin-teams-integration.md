---
title: Verwalten der Microsoft Teams-Integration in Business Central | Microsoft Docs
description: Verwalten Sie die Business Central-Integration in Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: 3c04dfb2f77eba906b2567ca9438849e1cc20861
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989376"
---
# <a name="managing-microsoft-teams-integration-with-business-central"></a><span data-ttu-id="93d37-103">Verwalten der Microsoft Teams-Integration in Business Central</span><span class="sxs-lookup"><span data-stu-id="93d37-103">Managing Microsoft Teams Integration with Business Central</span></span>

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

<span data-ttu-id="93d37-104">Dieser Artikel bietet einen Überblick darüber, was Sie als Administrator zur Steuerung der Microsoft Teams-Integration in [!INCLUDE [prodshort](includes/prodshort.md)] unternehmen können.</span><span class="sxs-lookup"><span data-stu-id="93d37-104">This article provides an overview of what you can do as an administrator to control Microsoft Teams integration with [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

## <a name="in-microsoft-teams"></a><span data-ttu-id="93d37-105">In Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="93d37-105">In Microsoft Teams</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="93d37-106">Mindestanforderungen</span><span class="sxs-lookup"><span data-stu-id="93d37-106">Minimum requirements</span></span>

<span data-ttu-id="93d37-107">In diesem Abschnitt werden die Mindestanforderungen für die Verwendung der [!INCLUDE [prodshort](includes/prodshort.md)]-App-Funktionen in Teams beschrieben.</span><span class="sxs-lookup"><span data-stu-id="93d37-107">This section describes the minimum requirements for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

- <span data-ttu-id="93d37-108">Erforderliche Lizenzen</span><span class="sxs-lookup"><span data-stu-id="93d37-108">Required licenses</span></span>

    <span data-ttu-id="93d37-109">Diese Tabelle gibt Ihnen einen Überblick über die Lizenzen, die für die Verwendung der [!INCLUDE [prodshort](includes/prodshort.md)]-App-Funktionen in Teams erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="93d37-109">This table gives you an overview of the licenses needed for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

    |<span data-ttu-id="93d37-110">Funktion</span><span class="sxs-lookup"><span data-stu-id="93d37-110">What</span></span>|<span data-ttu-id="93d37-111">Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="93d37-111">Teams license</span></span>|<span data-ttu-id="93d37-112">Business Central-Lizenz</span><span class="sxs-lookup"><span data-stu-id="93d37-112">Business Central license</span></span>|
    |----|---|---|
    |<span data-ttu-id="93d37-113">Einen Link zu einem [!INCLUDE [prodshort](includes/prodshort.md)]-Datensatz in eine Unterhaltung einfügen und ihn als Karte versenden.</span><span class="sxs-lookup"><span data-stu-id="93d37-113">Paste a link to a [!INCLUDE [prodshort](includes/prodshort.md)] record into a conversation, and send it as a card.</span></span>|<span data-ttu-id="93d37-114">![Häkchen](media/check.png "Aktivieren")</span><span class="sxs-lookup"><span data-stu-id="93d37-114">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="93d37-115">![Häkchen](media/check.png "Aktivieren")</span><span class="sxs-lookup"><span data-stu-id="93d37-115">![check mark](media/check.png "check")</span></span>|
    |<span data-ttu-id="93d37-116">Eine Karte eines [!INCLUDE [prodshort](includes/prodshort.md)]-Datensatzes in einer Unterhaltung anzeigen.</span><span class="sxs-lookup"><span data-stu-id="93d37-116">View a card of a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="93d37-117">![Häkchen](media/check.png "Aktivieren")</span><span class="sxs-lookup"><span data-stu-id="93d37-117">![check mark](media/check.png "check")</span></span>||
    |<span data-ttu-id="93d37-118">Weitere Details für eine Karte eines [!INCLUDE [prodshort](includes/prodshort.md)]-Datensatzes in einer Unterhaltung anzeigen.</span><span class="sxs-lookup"><span data-stu-id="93d37-118">View more details of card for a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="93d37-119">![Häkchen](media/check.png "Aktivieren")</span><span class="sxs-lookup"><span data-stu-id="93d37-119">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="93d37-120">![Häkchen](media/check.png "Aktivieren")</span><span class="sxs-lookup"><span data-stu-id="93d37-120">![check mark](media/check.png "check")</span></span>|

- <span data-ttu-id="93d37-121">URL-Vorschau zulassen</span><span class="sxs-lookup"><span data-stu-id="93d37-121">Allow URL previews</span></span>

    <span data-ttu-id="93d37-122">Die Richtlinieneinstellung **URL-Vorschau zulassen** muss aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="93d37-122">**Allow URL previews** policy setting must be turned on.</span></span> <span data-ttu-id="93d37-123">Andernfalls kann keine Karte für Business Central-Links generiert werden, die in eine Teams-Unterhaltung eingefügt werden.</span><span class="sxs-lookup"><span data-stu-id="93d37-123">Otherwise, a card can't be generated for Business Central links pasted into a Teams conversation.</span></span> <span data-ttu-id="93d37-124">Weitere Informationen zu dieser Einstellung finden Sie unter [Nachrichtenrichtlinien in Teams verwalten](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="93d37-124">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span>

### <a name="managing-the-business-central-app-optional"></a><span data-ttu-id="93d37-125">Verwalten der Business Central-App (optional)</span><span class="sxs-lookup"><span data-stu-id="93d37-125">Managing the Business Central app (optional)</span></span>

<span data-ttu-id="93d37-126">Als Teams-Administrator können Sie alle Apps für Ihre Organisation verwalten, einschließlich der [!INCLUDE [prodshort](includes/prodshort.md)]-App.</span><span class="sxs-lookup"><span data-stu-id="93d37-126">As a Teams administrator, you can manage all apps for your organization, including the [!INCLUDE [prodshort](includes/prodshort.md)] app.</span></span> <span data-ttu-id="93d37-127">Sie können die [!INCLUDE [prodshort](includes/prodshort.md)]-App für Ihr Unternehmen genehmigen oder installieren, die Installation der App durch Benutzer blockieren und vieles mehr.</span><span class="sxs-lookup"><span data-stu-id="93d37-127">You can approve or install the [!INCLUDE [prodshort](includes/prodshort.md)] app for your organization, block user's from installing the app, and more.</span></span>

<span data-ttu-id="93d37-128">Weitere Informationen finden Sie in den folgenden Artikeln in der Microsoft Teams-Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="93d37-128">For more information, see the following articles in the Microsoft Teams documentation:</span></span>

- [<span data-ttu-id="93d37-129">Ihre Apps im Microsoft Teams Admin Center verwalten</span><span class="sxs-lookup"><span data-stu-id="93d37-129">Manage your apps in the Microsoft Teams admin center</span></span>](https://docs.microsoft.com/MicrosoftTeams/manage-apps)
- [<span data-ttu-id="93d37-130">App-Einrichtungsrichtlinien in Microsoft Teams verwalten</span><span class="sxs-lookup"><span data-stu-id="93d37-130">Manage app setup policies in Microsoft Teams</span></span>](https://docs.microsoft.com/microsoftteams/teams-app-setup-policies)

## <a name="in-prodshort"></a><span data-ttu-id="93d37-131">In [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="93d37-131">In [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="93d37-132">Mindestanforderungen</span><span class="sxs-lookup"><span data-stu-id="93d37-132">Minimum requirements</span></span>

- <span data-ttu-id="93d37-133">[!INCLUDE [prodshort](includes/prodshort.md)]-Version:</span><span class="sxs-lookup"><span data-stu-id="93d37-133">[!INCLUDE [prodshort](includes/prodshort.md)] version:</span></span>

    <span data-ttu-id="93d37-134">[!INCLUDE [prodshort](includes/prodshort.md)] 2020 Veröffentlichungzyklus 2 (Version 17) oder höher.</span><span class="sxs-lookup"><span data-stu-id="93d37-134">[!INCLUDE [prodshort](includes/prodshort.md)] 2020 release wave 2 (version 17) or later.</span></span> <span data-ttu-id="93d37-135">Die Teams-Integration wird nur für [!INCLUDE [prodshort](includes/prodshort.md)] Online unterstützt, nicht für On-Premises.</span><span class="sxs-lookup"><span data-stu-id="93d37-135">Teams integration is only supported for [!INCLUDE [prodshort](includes/prodshort.md)] online; not on-premises.</span></span>

- <span data-ttu-id="93d37-136">Codeunit **2718 Seitenzusammenfassungsanbieter** wird als Webdienst veröffentlicht:</span><span class="sxs-lookup"><span data-stu-id="93d37-136">Codeunit **2718 Page Summary Provider** is published as a web service:</span></span>

    <span data-ttu-id="93d37-137">Diese Codeunit wird standardmäßig als Webdienst veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="93d37-137">This codeunit is published as a web service by default.</span></span> <span data-ttu-id="93d37-138">Die Codeunit ist Teil der [!INCLUDE [prodshort](includes/prodshort.md)]-Systemanwendung.</span><span class="sxs-lookup"><span data-stu-id="93d37-138">The codeunit is part of the [!INCLUDE [prodshort](includes/prodshort.md)] system application.</span></span> <span data-ttu-id="93d37-139">Sie wird verwendet, um die Felddaten für eine [!INCLUDE [prodshort](includes/prodshort.md)]-Seite abzurufen, die einer Teams-Unterhaltung hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="93d37-139">It's used to get the field data for a [!INCLUDE [prodshort](includes/prodshort.md)] page added to a Teams conversation.</span></span> 

- <span data-ttu-id="93d37-140">Benutzerberechtigungen:</span><span class="sxs-lookup"><span data-stu-id="93d37-140">User permissions:</span></span>

    <span data-ttu-id="93d37-141">Die Seiten und Daten, die Benutzer in einer Teams-Unterhaltung anzeigen und bearbeiten können, werden größtenteils durch deren Berechtigungen in [!INCLUDE [prodshort](includes/prodshort.md)] gesteuert.</span><span class="sxs-lookup"><span data-stu-id="93d37-141">For the most part, the pages and data that users can view and edit in a Teams conversation is controlled by their permissions in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>
    
    - <span data-ttu-id="93d37-142">Um einen [!INCLUDE [prodshort](includes/prodshort.md)]-Link in eine Teams-Unterhaltung einzufügen und diesen zu einer Karte zu erweitern, müssen Benutzer mindestens über die Leseberechtigung für die Seite und ihre Daten verfügen.</span><span class="sxs-lookup"><span data-stu-id="93d37-142">To paste a [!INCLUDE [prodshort](includes/prodshort.md)] link into a Teams conversation and have it expand into a card, users must have at least read permission on the page and its data.</span></span>
    - <span data-ttu-id="93d37-143">Sobald eine Karte in eine Unterhaltung übermittelt wurde, kann jeder Benutzer in dieser Unterhaltung diese Karte ohne Berechtigungen für Business Central anzeigen.</span><span class="sxs-lookup"><span data-stu-id="93d37-143">Once a card is submitted into a conversation, any user in that conversation can view that card without permission to Business Central.</span></span>
    - <span data-ttu-id="93d37-144">Um weitere Details für eine Karte anzuzeigen oder den Datensatz in [!INCLUDE [prodshort](includes/prodshort.md)] zu öffnen, müssen Benutzer über Leseberechtigung für die Seite und ihre Daten verfügen.</span><span class="sxs-lookup"><span data-stu-id="93d37-144">To view more details for a card or open the record in [!INCLUDE [prodshort](includes/prodshort.md)], users must have read permission on the page and its data.</span></span>
    - <span data-ttu-id="93d37-145">Um Daten zu ändern, benötigen Benutzer Änderungsberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="93d37-145">To change data, user's need modify permissions.</span></span>
    
    <span data-ttu-id="93d37-146">Weitere Informationen zu Berechtigungen finden Sie unter [Berechtigungen an Benutzer und Gruppen zuweisen](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="93d37-146">For information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="93d37-147">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="93d37-147">See Also</span></span>
[<span data-ttu-id="93d37-148">Übersicht über die Integration von Business Central und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="93d37-148">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="93d37-149">[Die [!INCLUDE [prodshort](includes/prodshort.md)]-App für Microsoft Teams installieren](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="93d37-149">[Install the [!INCLUDE [prodshort](includes/prodshort.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="93d37-150">Entwicklung für die Teams-Integration</span><span class="sxs-lookup"><span data-stu-id="93d37-150">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[<span data-ttu-id="93d37-151">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="93d37-151">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  