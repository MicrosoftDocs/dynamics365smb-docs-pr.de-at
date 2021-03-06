---
title: Einrichten von eingehenden Belegen| Microsoft Docs
description: Verwenden Sie die Funktion der eingehenden Belege, um elektronische Belege zu erstellen, verwalten Sie OCRaufgaben, importieren Sie Rechnungen und wandeln Sie Bilddateien um.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3a43c32d90a7c27af56ed55a4625b3dc3faf498b
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754909"
---
# <a name="set-up-incoming-documents"></a>Einrichten von eingehenden Belegen

Wenn Sie Fibu Buch.-Blattzeilen für eingehende Belegdatensätze erstellen, müssen Sie auf der Seite **Einrichtung für eingehende Belege** angeben, welche Buch.-Blattvorlage und welches Buch.-Blatt verwendet werden sollen.

Wenn Sie möchten, dass Benutzer Rechnungen oder Journalzeilen anhand von Eingangsbelegen nur dann erstellen können, wenn diese genehmigt sind, müssen Sie Workflow-Genehmiger einrichten.

Um PDF und Bilddateien in elektronische Belege umzuwandeln, die in Belegdatensätze in Project '[!INCLUDE[prod_short](includes/prod_short.md)]' konvertiert werden, müssen Sie die OCR-Funktion einrichten und den Dienst aktivieren. Wählen Sie ein Servicepaket, das für Ihre Organisation und/oder Ihr Land/Ihre Region geeignet ist. Alternativ können Sie Einträge manuell erstellen, um die externen Dokumente darzustellen.  

Wenn die Funktion „Eingehende Belege“ eingerichtet ist, können Sie verschiedene Funktionen zum Überprüfen von Ausgabenbelegen, Verwalten von OCR-Aufgaben und Konvertieren von eingehenden Belegen, manuell oder automatisch, in den entsprechenden Belegen oder Buch.-Blattzeilen verwenden. Die externen Dateien können jeder Prozessphase zugeordnet werden, auch gebuchten Belegen und den resultierenden Kreditoren-, Debitoren- und Sachposten. Weitere Informationen finden Sie unter [Eingehende Belege verarbeiten](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>So richten Sie die Funktion „Eingehende Belege“ ein

1. Wählen Sie das Symbol ![Glühbirne, die die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell Me-Funktion") aus, geben Sie **Eingehenden Beleg einrichten** ein, und wählen Sie dann den zugehörigen Link.
2. Füllen Sie die Felder je nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Im Rahmen der Einrichtung müssen Sie entscheiden, ob Sie die Genehmigung eingehender Belege benötigen. Um eine Genehmigung anzufordern, müssen Sie Genehmiger und Genehmigungsworkflows einrichten. Wenn Ihre Organisation nicht beabsichtigt, eine Genehmigung anzufordern, können Sie den nächsten Abschnitt überspringen.  

Schließlich müssen Sie, wenn Sie einen Dienst zur Konvertierung von PDF- oder Bilddateien verwenden, die eingehende Belege darstellen, diesen einrichten. Andernfalls können Sie diesen Abschnitt auch überspringen.  

## <a name="to-set-up-approvers-of-incoming-document-records"></a>So richten Sie Genehmiger für eingehende Belege ein

Richten Sie optional einen Genehmigungsprozess für die eingehenden Dokumente ein. Genehmiger von eingehenden Belegen müssen als Genehmigungsworkflow-Benutzer eingerichtet werden.

Bevor Sie Workflows erstellen können, die Genehmigungsschritte betreffen, müssen Sie die Workflowbenutzer einrichten, die von den Genehmigungsprozessen betroffen sind. Auf der Seite **Genehmigungsbenutzereinrichtung** müssen Sie zusätzlich Grenzbeträge für bestimmte Arten von Anforderungen festlegen und Ersatzgenehmiger definieren, an die Genehmigungsanforderungen delegiert werden, wenn der ursprüngliche Genehmiger abwesend ist. Weitere Informationen finden Sie unter [Einrichten von Genehmigungsbenutzern.](across-how-to-set-up-approval-users.md)

## <a name="to-set-up-an-ocr-service"></a>So richten Sie einen OCR-Service ein

1. Wählen Sie das Symbol ![Glühbirne, die die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell Me-Funktion") aus, geben Sie **OCR-Serviceeinrichtung** ein und wählen Sie dann den entsprechenden Link.
2. Füllen Sie die Felder je nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> Sie informieren Daten werden verschlüsselt automatisch an.

Weitere Informationen finden Sie unter [Verwenden von OCR, um PDF und Bilddateien in elektronische Belege umzuwandeln](across-how-use-ocr-pdf-images-files.md).  

## <a name="see-also"></a>Siehe auch

[Eingehende Belege verarbeiten](across-process-income-documents.md)  
[Eingehende Belege](across-income-documents.md)  
[Einkauf](purchasing-manage-purchasing.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]