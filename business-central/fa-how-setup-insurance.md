---
title: Abschreibungsrsicherung einrichten| Microsoft Docs
description: Um die Abdeckung der Anlagenversicherung zu verwalten, müssen Sie pro Versicherung einige allgemeine Versicherungsinformationen und eine Versicherungskarte einrichten.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: c5c9af3a076647380e2f6bed8ef7d0a55c3d8efe
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749310"
---
# <a name="set-up-fixed-asset-insurance"></a>Um Anlagenversicherung einzurichten:
Um die Abdeckung der Anlagenversicherung zu verwalten, müssen Sie pro Versicherung einige allgemeine Versicherungsinformationen und eine Versicherungskarte einrichten.

## <a name="to-set-up-general-insurance-information"></a>So richten Sie allgemeine Versicherungsinformationen ein
Um die Versicherungsfunktionen in [!INCLUDE[prod_short](includes/prod_short.md)]  verwenden zu können, müssen Sie einige allgemeine Versicherungsinformationen einrichten.  

1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Anlagen Einrichtung** ein und wählen Sie dann den entsprechenden Link.  
2. Füllen Sie die Felder je nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-insurance-types"></a>So richten Sie Versicherungsarten ein
Sie können die Versicherungspolicen in Kategorien gruppieren, beispielsweise für Diebstahl- und Feuerversicherungen. Die Versicherungsarten werden auf der Versicherungskarte verwendet.

1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Versicherungstypen** ein und wählen Sie dann den entsprechenden Link.  
2. Füllen Sie die Felder je nach Bedarf aus.

## <a name="to-set-up-insurance-cards"></a>So richten Sie Versicherungskarten ein
Sie können die gesammelten Informationen über die einzelnen Versicherungspolicen auf der Versicherungskarte eingeben.  

1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Versicherung** ein und wählen Sie dann den entsprechenden Link.  
2. Wählen Sie auf der Seite **Versicherung** die Aktion **Neu** aus, um eine neue Karte für eine Versicherungspolice zu erstellen.  
3. Füllen Sie die Felder je nach Bedarf aus.

## <a name="to-set-up-insurance-journal-templates"></a>So richten Sie Versicherungs Buch.-Blattvorlagen ein
[!INCLUDE[prod_short](includes/prod_short.md)] erstellt automatisch eine Versicherungs-Buch.-Blattvorlage, wenn Sie zum ersten Mal die Seite **Versicherungs Buch.-Blatt** öffnen; Sie können aber zusätzliche Vorlagen einrichten. Weitere Informationen finden Sie unter [Arbeiten mit Fibu Buch.-Blättern](ui-work-general-journals.md)  

1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Vers. Buch.-Blattvorlagen** ein und wählen Sie dann den entsprechenden Link.  
2. Füllen Sie die Felder je nach Bedarf aus.

## <a name="to-set-up-insurance-journal-batches"></a>So richten Sie Versicherungs Buch.-Blattnamen ein
Sie können zusätzliche Namen in einer Versicherungs Buch.-Blattvorlage einrichten. Die Werte in dem Buch.-Blattnamen werden als Vorgabewerte verwendet, wenn die Felder in den Buch.-Blattzeilen nicht ausgefüllt sind. Weitere Informationen finden Sie unter [Arbeiten mit Fibu Buch.-Blättern](ui-work-general-journals.md)  

1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Vers. Buch.-Blattvorlagen** ein und wählen Sie dann den entsprechenden Link.  
2. Wählen Sie eine Vers. Buch.-Blattvorlage und dann die Aktion **Buch.-Blattnamen** aus.
3. Füllen Sie auf der Seite **Versicherung Buch.-Blattnamen** die notwendigen Felder aus.

> [!NOTE]  
>   Nummern haben in Buch.-Blattnamen eine spezielle Aufgabe. Wenn die Buch.-Blattvorlage oder der Buch.-Blattname eine Nummer enthält, wird diese beim Buchen des Buch.-Blatts automatisch um eins hochgezählt. Wenn z. B. HH1 in dem Feld **Name** verwendet wurde, ändert sich der Name auf HH2, nachdem das Buch.-Blatt HH1 gebucht wurde.

## <a name="see-also"></a>Siehe auch
[Anlagen einrichten](fa-setup.md)  
[Anlagen](fa-manage.md)  
[Finanzen](finance.md)  
[Erste Schritte](product-get-started.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]