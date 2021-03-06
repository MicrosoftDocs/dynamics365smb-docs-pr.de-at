---
title: Einrichten von Workflows
description: Sie können Workflows einrichten und verwenden, die Geschäftsprozessaufgaben von verschiedenen Benutzern verbinden. Erfahren Sie mehr über die verschiedenen Schritte, die Sie unternehmen müssen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/14/2020
ms.author: edupont
ms.openlocfilehash: a104065d8f52ca9d1bb9221cd43917253c640ca4
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754252"
---
# <a name="set-up-workflows"></a>Einrichten von Workflows

Sie können Workflows einrichten und verwenden, die Geschäftsprozessaufgaben von verschiedenen Benutzern verbinden. Systemaufgaben, wie automatische Buchung, können als Schritte in Workflows berücksichtigt werden, vor oder nach Benutzeraufgaben. Die Anforderung oder Bewilligung von Genehmigungen zum Erstellen neuer Datensätze sind typische Workflowschritte. Weitere Informationen erhalten Sie unter [Workflows verwenden](across-use-workflows.md).  

 Bevor Sie beginnen, Workflows zu verwenden, müssen Sie Workflowbenutzer und Genehmigungsbenutzer einrichten und angeben, wie Benutzer Benachrichtigungen über Workflowschritte empfangen sollen. Dann müssen Sie Workflows erstellen und möglicherweise zuvor Codeanpassungen vornehmen.  

 Auf der Seite **Workflow** können Sie einen Workflow erstellen, indem Sie die entsprechenden Schritte in den Zeilen auflisten. Jeder Schritt besteht aus einem durch Ereignisbedingungen moderiertem Workflowereignis und einer durch Antwortoptionen moderierten Workflowantwort. Sie definieren Workflowschritte, indem Sie die Felder in Workflowzeilen mit Ereignis- und Antwortwerten aus festen Listen ausfüllen, die die Workflowszenarien darstellen, die durch den Anwendungscode unterstützt werden.  

 Wenn ein Szenario ein Workflowereignis oder -antwort benötigt, die nicht unterstützt wird, muss ein Microsoft-Partner diese implementieren, indem er den Workflow mithilfe von Power Automate anpasst. Weitere Informationen finden Sie unter [Verwenden von [!INCLUDE[prod_short](includes/prod_short.md)] in einem automatisierten Workflow](across-how-use-financials-data-source-flow.md) oder [Veranstaltungen in AL](/dynamics365/business-central/dev-itpro/developer/devenv-events-in-al) in der Entwicklerhilfe.

 In der folgenden Tabelle wird eine Reihe von Aufgaben mit Verknüpfungen zu den beschriebenen Themen erläutert  

|**Aufgabe**|**Siehe**|  
|------------|-------------|  
|Einrichten von Workflowbenutzern und Benutzergruppen|[Einrichten von Workflowbenutzern](across-how-to-set-up-workflow-users.md)|  
|Richten Sie Workflowbenutzer ein, die an den Genehmigungsworkflows teilnehmen.|[Genehmigungsbenutzer einrichten](across-how-to-set-up-approval-users.md)|  
|Geben Sie an, wie Workflowbenutzer über Workflowschritte (einschließlich Genehmigungsanforderungen) benachrichtigt werden.|[Einrichten von Workflowbenachrichtigungen](across-setting-up-workflow-notifications.md)|  
|Geben Sie an, ob Benutzer per E-Mail oder Notiz benachrichtigt werden sollen und wie häufig Benachrichtigungen gebucht werden sollen.|[Angeben des Zeitpunkts und der Art des Empfangs von Benachrichtigungen](across-how-to-specify-when-and-how-to-receive-notifications.md)|  
|Wenn Sie möchten, können Sie den Inhalt der E-Mail-Benachrichtigung anpassen, indem Sie Bericht 1320, Benachrichtigungs-E-Mail ändern.|[Erstellen und Ändern benutzerdefinierter Berichtslayouts](ui-how-create-custom-report-layout.md)|  
|Richten Sie einen SMTP-Server so ein, dass die E-Mail-Kommunikation mit [!INCLUDE[prod_short](includes/prod_short.md)] aktiviert ist.|[E-Mail einrichten](admin-how-setup-email.md)|
|Geben Sie die verschiedenen Schritte eines Workflows mithilfe von Verbindungsworkflowereignissen mit Workflowantworten an.|[Erstellen eines Workflows](across-how-to-create-workflows.md)|  
|Verwenden Sie Workflowvorlagen, um neue Workflows zu erstellen.|[Erstellen von Workflows aus Workflowvorlagen](across-how-to-create-workflows-from-workflow-templates.md)|  
|Teilen Sie Workflows mit anderen [!INCLUDE[prod_short](includes/prod_short.md)]-Datenbanken.|[Exportieren und Importieren von Workflows](across-how-to-export-and-import-workflows.md)|  
|Erfahren Sie anhand eines vollständigen Ablaufs, wie Sie einen Workflow zur Genehmigung von Verkaufsunterlagen einrichten.|[Exemplarische Vorgehensweise: Einrichten und Nutzen eines Einkaufsanfrage-Genehmigungsworkflows](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)|  

## <a name="example-of-an-approval-workflow"></a>Beispiel eines Genehmigungsworkflows
In diesem Video wird gezeigt, wie ein Workflow eingerichtet wird, bei dem eine Person die Genehmigung einer anderen Person anfordern muss, bevor sie Informationen zu einem vorhandenen Kunden ändern oder einen neuen Kunden erstellen kann.  
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4jzHI?rel=0]

## <a name="see-also"></a>Siehe auch  
 [Verwenden von Workflows](across-use-workflows.md)   
 [Workflow](across-workflow.md)   
 [Exemplarische Vorgehensweise: Einrichten und Nutzen eines Einkaufsanfrage-Genehmigungsworkflows](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
 [Arbeiten mit  Business Central](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]