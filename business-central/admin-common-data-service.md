---
title: Verwendung von Common Data Service
description: Einführung in Common Data Service und seine Komponenten.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 10/01/2020
ms.openlocfilehash: 85823e93b1d239bf4e59ec6a8872cdc4a2cef9c1
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911597"
---
# <a name="integrating-with-common-data-service"></a><span data-ttu-id="8debf-103">Integrieren in Common Data Service</span><span class="sxs-lookup"><span data-stu-id="8debf-103">Integrating with Common Data Service</span></span>

<span data-ttu-id="8debf-104">Geschäftsanwendungen verwenden häufig Daten aus mehr als einer Quelle.</span><span class="sxs-lookup"><span data-stu-id="8debf-104">Business apps often use data from more than one source.</span></span> [!INCLUDE[d365fin](includes/cds_long_md.md)] <span data-ttu-id="8debf-105">kombiniert Daten in einem einzigen Satz von Logik, der es einfacher macht, andere Dynamics 365-Anwendungen, wie [!INCLUDE[crm_md](includes/crm_md.md)] oder Ihre eigene Anwendung, die auf [!INCLUDE[d365fin](includes/cds_long_md.md)] aufbaut, mit [!INCLUDE[d365fin_md](includes/d365fin_md.md)] zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="8debf-105">combines data into a single set of logic that makes it easier to connect other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)] or your own application built on top of [!INCLUDE[d365fin](includes/cds_long_md.md)], to [!INCLUDE[d365fin_md](includes/d365fin_md.md)].</span></span> <span data-ttu-id="8debf-106">Für weitere Informationen über [!INCLUDE[d365fin](includes/cds_long_md.md)] siehe [Was ist Common Data Service?](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro)</span><span class="sxs-lookup"><span data-stu-id="8debf-106">For more information about [!INCLUDE[d365fin](includes/cds_long_md.md)], see [What is Common Data Service?](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro)</span></span>

<span data-ttu-id="8debf-107">Die folgenden Schritte bieten einen Überblick über die Schritte für die Integration von [!INCLUDE[d365fin](includes/cds_long_md.md)] mit [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8debf-107">The following steps provide an overview of the steps to integrate [!INCLUDE[d365fin](includes/cds_long_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

> [!Note]  
> <span data-ttu-id="8debf-108">Für diese Aufgaben ist die Sicherheitsrolle des **Systemadministrators** in [!INCLUDE[d365fin](includes/cds_long_md.md)] und [!INCLUDE[d365fin](includes/d365fin_md.md)] erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8debf-108">These tasks require the **System Administrator** security role in [!INCLUDE[d365fin](includes/cds_long_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

1. <span data-ttu-id="8debf-109">Weisen Sie Lizenzen für [!INCLUDE[d365fin](includes/cds_long_md.md)] den [!INCLUDE[d365fin](includes/d365fin_md.md)]-Benutzern zu, die die integrierten Apps verwenden werden.</span><span class="sxs-lookup"><span data-stu-id="8debf-109">Assign licenses for [!INCLUDE[d365fin](includes/cds_long_md.md)] to the [!INCLUDE[d365fin](includes/d365fin_md.md)] users who will use the integrated apps.</span></span>

2. <span data-ttu-id="8debf-110">Richten Sie eine Verbindung mit [!INCLUDE[d365fin](includes/cds_long_md.md)] ein.</span><span class="sxs-lookup"><span data-stu-id="8debf-110">Set up a connection to [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="8debf-111">Weitere Informationen finden Sie unter [Verbindung zu Common Data Service](admin-how-to-set-up-a-dynamics-crm-connection.md).</span><span class="sxs-lookup"><span data-stu-id="8debf-111">For more information, see [Connect to Common Data Service](admin-how-to-set-up-a-dynamics-crm-connection.md).</span></span>  

3. <span data-ttu-id="8debf-112">Synchronisieren Sie die Daten zwischen den Apps.</span><span class="sxs-lookup"><span data-stu-id="8debf-112">Synchronize data between the apps.</span></span> <span data-ttu-id="8debf-113">Weitere Informationen finden Sie unter [Synchronisieren von Business Central und Common Data Service](admin-synchronizing-business-central-and-sales.md).</span><span class="sxs-lookup"><span data-stu-id="8debf-113">For more information, see [Synchronizing Business Central and Common Data Service](admin-synchronizing-business-central-and-sales.md).</span></span> 

## <a name="getting-started-with-d365fin"></a><span data-ttu-id="8debf-114">Erste Schritte mit [!INCLUDE[d365fin](includes/cds_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="8debf-114">Getting Started with [!INCLUDE[d365fin](includes/cds_long_md.md)]</span></span>
<span data-ttu-id="8debf-115">Um mit [!INCLUDE[d365fin](includes/cds_long_md.md)] zu beginnen, benötigen Sie ein Microsoft Power Apps-Konto.</span><span class="sxs-lookup"><span data-stu-id="8debf-115">To get started with [!INCLUDE[d365fin](includes/cds_long_md.md)] you will need a Microsoft Power Apps account.</span></span> <span data-ttu-id="8debf-116">Wenn Sie noch nicht über ein Power Apps-Konto verfügen, können Sie ein kostenloses Konto erhalten, indem Sie [powerapps.com](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) besuchen und den Link **Kostenlos einsteigen** wählen.</span><span class="sxs-lookup"><span data-stu-id="8debf-116">If you do not already have a Power Apps account, you can get one for free by visiting [powerapps.com](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) and choosing the **Get started free** link.</span></span> <span data-ttu-id="8debf-117">Weitere Informationen zu den ersten Schritten mit [!INCLUDE[d365fin](includes/cds_long_md.md)] finden Sie im Modul [Erste Schritte mit Common Data Service](https://docs.microsoft.com/learn/modules/get-started-with-powerapps-common-data-service/) von Microsoft Learn.</span><span class="sxs-lookup"><span data-stu-id="8debf-117">To learn more about how to get started with [!INCLUDE[d365fin](includes/cds_long_md.md)], see the [Get started with Common Data Service](https://docs.microsoft.com/learn/modules/get-started-with-powerapps-common-data-service/) module from Microsft Learn.</span></span>

## <a name="bi-directional-or-uni-directional-data-synchronization"></a><span data-ttu-id="8debf-118">Bidirektionale oder unidirektionale Datensynchronisation</span><span class="sxs-lookup"><span data-stu-id="8debf-118">Bi-Directional or Uni-directional Data Synchronization</span></span>
<span data-ttu-id="8debf-119">Je nach Ihren Geschäftsanforderungen können Sie die Integration so einrichten, dass Daten entweder mit einer Dynamics 365-Geschäftsanwendung oder von einer Dynamics 365-Geschäftsanwendung zu einer anderen synchronisiert werden oder in beiden Richtungen in nahezu Echtzeit durch [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8debf-119">Depending on your business needs, you can set up the integration to synchronize data either to or from one Dynamics 365 business app to another, or in both directions in near-real time through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="8debf-120">Wenn Sie z.B. [!INCLUDE[d365fin](includes/d365fin_md.md)] mit [!INCLUDE[crm_md](includes/crm_md.md)] bis [!INCLUDE[d365fin](includes/cds_long_md.md)] integrieren, kann ein Kreditor einen Debitorenauftrag in [!INCLUDE[crm_md](includes/crm_md.md)] erstellen, und der Auftrag wird mit [!INCLUDE[d365fin](includes/d365fin_md.md)] synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="8debf-120">For example, if you integrate [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)] through [!INCLUDE[d365fin](includes/cds_long_md.md)], a salesperson can create a sales order in [!INCLUDE[crm_md](includes/crm_md.md)] and the order will be synchronized to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="8debf-121">Umgekehrt kann der Verkäufer von [!INCLUDE[crm_md](includes/crm_md.md)] aus Informationen von [!INCLUDE[d365fin](includes/d365fin_md.md)] über die Verfügbarkeit des Artikels auf der Bestellung einsehen.</span><span class="sxs-lookup"><span data-stu-id="8debf-121">Conversely, from [!INCLUDE[crm_md](includes/crm_md.md)], the salesperson can view information from [!INCLUDE[d365fin](includes/d365fin_md.md)] about the availability of the item on the order.</span></span> 

## <a name="standard-and-custom-entities"></a><span data-ttu-id="8debf-122">Standard- und benutzerdefinierte Entitäten</span><span class="sxs-lookup"><span data-stu-id="8debf-122">Standard and Custom Entities</span></span>
[!INCLUDE[d365fin](includes/cds_long_md.md)] <span data-ttu-id="8debf-123">speichert Daten sicher in einem Satz von Entitäten, das sind Datensätze, ähnlich wie eine Tabelle Daten in einer Datenbank speichert.</span><span class="sxs-lookup"><span data-stu-id="8debf-123">securely stores data in a set of entities, which are sets of records similar to how a table stores data within a database.</span></span> [!INCLUDE[d365fin](includes/cds_long_md.md)] <span data-ttu-id="8debf-124">enthält einen Basissatz von Standardentitäten, die typische Szenarien abdecken, aber Sie können auch benutzerdefinierte Entitäten erstellen, die spezifisch für Ihre Organisation sind.</span><span class="sxs-lookup"><span data-stu-id="8debf-124">includes a base set of standard entities that cover typical scenarios, but you can also create custom entities specific to your organization.</span></span> <span data-ttu-id="8debf-125">In [!INCLUDE[d365fin](includes/d365fin_md.md)] können Sie Standard- und benutzerdefinierte Entitäten anzeigen, die auf der Seite Integrationstabellenzuordnungen synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="8debf-125">In [!INCLUDE[d365fin](includes/d365fin_md.md)], you can view standard and custom entities being synchronized on the Integration Table Mappings page.</span></span>

## <a name="about-the-base-cds-integration-solution"></a><span data-ttu-id="8debf-126">Über die CDS-Basisintegrationslösung</span><span class="sxs-lookup"><span data-stu-id="8debf-126">About the Base CDS Integration Solution</span></span>

<span data-ttu-id="8debf-127">Die CDS-Basisintegrationslösung ist eine Schlüsselkomponente der Integration.</span><span class="sxs-lookup"><span data-stu-id="8debf-127">The Base CDS Integration Solution is a key component of the integration.</span></span> <span data-ttu-id="8debf-128">Die Lösung fügt den Benutzerkonten für die Integration die erforderlichen Rollen und Zugriffsebenen hinzu, und sie erstellt Einheiten, die für die Zuordnung von [!INCLUDE[d365fin](includes/d365fin_md.md)] Unternehmen zu Geschäftseinheit in [!INCLUDE[d365fin](includes/cds_long_md.md)] erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8debf-128">The solution adds the required roles and access levels to the user accounts for the integration, and it creates entities needed to map [!INCLUDE[d365fin](includes/d365fin_md.md)] company to business unit in [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> 

<span data-ttu-id="8debf-129">Standardmäßig importiert die unterstützte Einrichtung **[!INCLUDE[d365fin](includes/cds_long_md.md)]-Verbindung einrichten** die Lösung.</span><span class="sxs-lookup"><span data-stu-id="8debf-129">By default, the **Set up [!INCLUDE[d365fin](includes/cds_long_md.md)] connection** assisted setup guide will import the solution.</span></span> <span data-ttu-id="8debf-130">Dazu verwendet der Einrichtungsleitfaden ein Administrator-Benutzerkonto, das Sie angeben.</span><span class="sxs-lookup"><span data-stu-id="8debf-130">To do that, the setup guide uses an administrator user account that you specify.</span></span> <span data-ttu-id="8debf-131">Dieses Konto muss ein gültiger Benutzer in [!INCLUDE[d365fin](includes/cds_long_md.md)] mit der folgenden Sicherheitsrolle sein:</span><span class="sxs-lookup"><span data-stu-id="8debf-131">This account must be a valid user in [!INCLUDE[d365fin](includes/cds_long_md.md)] with the following security role:</span></span>

* <span data-ttu-id="8debf-132">Systemadministrator</span><span class="sxs-lookup"><span data-stu-id="8debf-132">System Administrator</span></span>  

<span data-ttu-id="8debf-133">Weitere Informationen finden Sie unter [Benutzerkonten für die Integration einrichten mit [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) und [Benutzer in Microsoft Dynamics 365 (online) anlegen und Sicherheitsrollen zuweisen](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles).</span><span class="sxs-lookup"><span data-stu-id="8debf-133">For more information, see [Setting Up User Accounts for Integrating with [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) and [Create users in Microsoft Dynamics 365 (online) and assign security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles).</span></span> 

<span data-ttu-id="8debf-134">Das Administratorkonto wird aufgrund von Konfigurationsänderungen, die die Basis-CDS-Lösung in [!INCLUDE[d365fin](includes/cds_long_md.md)] vornimmt, während der Einrichtung nur einmal verwendet.</span><span class="sxs-lookup"><span data-stu-id="8debf-134">The administrator account is used only one time during the setup due to configuration changes Base CDS Solution is making in [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="8debf-135">Nachdem die Lösung importiert wurde, wird das Konto nicht mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="8debf-135">After the solution is imported the account is no longer needed.</span></span> <span data-ttu-id="8debf-136">Bei der Integration wird dann weiterhin das Benutzerkonto verwendet, das automatisch speziell für die Integration erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="8debf-136">Integration will continue to use the user account that is automatically created specifically for the integration.</span></span>

<span data-ttu-id="8debf-137">Zusätzlich zur Anpassung von [!INCLUDE[d365fin](includes/cds_long_md.md)] erstellt die Lösung auch die folgenden Rollen in [!INCLUDE[d365fin](includes/cds_long_md.md)] für die Integration:</span><span class="sxs-lookup"><span data-stu-id="8debf-137">In addition to customizing [!INCLUDE[d365fin](includes/cds_long_md.md)], the solution also creates the following roles in [!INCLUDE[d365fin](includes/cds_long_md.md)] for the integration:</span></span>

* <span data-ttu-id="8debf-138">**Integrationsadministrator**  – Ermöglicht es Benutzern, die Verbindung zwischen [!INCLUDE[d365fin](includes/d365fin_md.md)] und [!INCLUDE[d365fin](includes/cds_long_md.md)] zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="8debf-138">**Integration Administrator** - Allows users to manage the connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="8debf-139">Normalerweise wird diese nur dem automatisch erstellten Benutzerkonto für die Synchronisierung zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="8debf-139">Typically, this is assigned only to the automatically created user account for synchronization.</span></span>  
* <span data-ttu-id="8debf-140">**Integrationsbenutzer**  – Ermöglicht es Benutzern, auf synchronisierte Daten zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="8debf-140">**Integration User** - Allows users to access synchronized data.</span></span> <span data-ttu-id="8debf-141">In der Regel wird dies dem automatisch erstellten Benutzerkonto für die Synchronisierung und anderen Benutzern zugewiesen, die die synchronisierten Daten anzeigen oder auf sie zugreifen müssen.</span><span class="sxs-lookup"><span data-stu-id="8debf-141">Typically, this is assigned to the automatically created user account for synchronization and other users who need to view or access the synchronized data.</span></span>

<span data-ttu-id="8debf-142">Weitere Informationen zu den einzelnen Rollen, z. B. zu Berechtigungen und Zugriffsebenen, finden Sie unter [Einrichten von Benutzerkonten für die Integration mit [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).</span><span class="sxs-lookup"><span data-stu-id="8debf-142">For details about each role, such as the permissions and access levels, see [Setting Up User Accounts for Integrating with [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).</span></span>

<span data-ttu-id="8debf-143">Während des Verbindungsaufbaus werden Integrationstabellenzuordnungen erstellt, die zur Datensynchronisation benötigt werden.</span><span class="sxs-lookup"><span data-stu-id="8debf-143">During connection setup, integration table mappings that are needed to synchronize data, are created.</span></span> <span data-ttu-id="8debf-144">Entitäten in Common Data Service werden Tabellen und Tabellenfeldern in Business Central durch Integrationstabellen zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="8debf-144">Entities in Common Data Service are mapped to tables and table fields in Business Central through integration tables.</span></span> <span data-ttu-id="8debf-145">Weitere Informationen finden Sie unter [Standard Entitätszuordnung für die Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-entity-mapping-for-synchronization).</span><span class="sxs-lookup"><span data-stu-id="8debf-145">For more information, see [Standard Entity Mapping for Synchronization](admin-synchronizing-business-central-and-sales.md#standard-entity-mapping-for-synchronization).</span></span>

## <a name="see-also"></a><span data-ttu-id="8debf-146">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8debf-146">See Also</span></span>
[<span data-ttu-id="8debf-147">Dateneigentumsmodelle</span><span class="sxs-lookup"><span data-stu-id="8debf-147">Data Ownership Models</span></span>](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Common Data Service](docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-custom-cds-integration) -->


