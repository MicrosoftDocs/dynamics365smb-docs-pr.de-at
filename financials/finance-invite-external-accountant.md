---
title: "Fügen Sie Ihren externen Buchhalter Ihrem Financials hinzu | Microsoft Docs"
description: "Erfahren Sie, wie Sie den externen Buchhalter zu Ihrem Dynamics 365 Business edition einladen können."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 11/10/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 9769d4b1e34da62290cc97de291462ee2d22c747
ms.contentlocale: de-at
ms.lasthandoff: 11/10/2017

---
# <a name="inviting-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Externen Buchhalter einladen zu Ihrem [!INCLUDE[d365fin](includes/d365fin_md.md)]
Wenn Sie eines externen Buchhalter verwenden, um Ihre Buch und Berichte zu verwalten, können Sie sie für Ihr [!INCLUDE[d365fin](includes/d365fin_md.md)] einladen, damit sie mit Ihnen an Ihren steuerlichen Daten arbeiten.

Sobald Ihr Buchhalter zu den verwendeten [!INCLUDE[d365fin](includes/d365fin_md.md)] Zugriff hat, können sie das Rollencenter **Buchhalter** verwenden, das Zugriff auf den relevantsten Fenstern für ihre Arbeit gibt.  

> [!NOTE]  
>  Diese Funktionen erfordert, dass die Benutzeroberfläche in **Suite** festgelegt wird. Weitere Informationen finden Sie unter [Anpassen Ihrer Dynamics 365 Experience](ui-experiences.md).  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a>Ihren Buchhalter einladen zu Ihrem [!INCLUDE[d365fin](includes/d365fin_md.md)]
In der neuesten Version von [!INCLUDE[d365fin](includes/d365fin_md.md)] machen wir es Ihnen ganz einfach, Ihren externen Buchhalter einzuladen. Öffnen Sie einfach das Fenster **Benutzer** und wählen Sie im Band die Aktion **Externen Buchhalter einladen**. Es wird eine E-Mail für Sie vorbereitet. Sie tragen einfach nur die E-Mail-Adresse Ihres Buchhalters ein und senden die Einladung ab.  

![Ihren Buchhalter einladen](./media/finance-invite-accountant/invite-accountant.png)

> [!TIP]  
>  Dies setzt voraus, dass Sie SMPT-E-Mail eingerichtet haben. Dies können Sie selbst machen, oder Ihren [!INCLUDE[d365fin](includes/d365fin_md.md)]-Partner darum bitten. Zudem müssen als [!INCLUDE[d365fin](includes/d365fin_md.md)] Benutzeradministrator, nicht als der Geschäftsinhaber oder andere Benutzer angemeldet sind. Schließlich müssen Sie das Testunternehmen verlassen haben, sodass Sie einen Azure Active Directory- Azure Active Directory haben.  

> [!IMPORTANT]  
>  Die E-Mail-Adresse des Buchhalters muss eine Arbeitsadresse sein, die auf einem Active Directory basiert. Wenn der Buchhalter eine andere Art von E-Mail verwendet, kann die Einladung nicht gesendet werden.  

### <a name="separate-license"></a>Lizenzen trennen
Hinter den Kulissen wird der Buchhalter Ihrem Active Directory-Mandanten hinzugefügt. Ihr Administrator kann überprüfen, ob der Buchhalter die Einladung akzeptiert und der richtigen Lizenz hinzugefügt wird. Die Schritte dazu hängen von der Art des Kontos ab, das Sie verwendet haben, als Sie sich bei [!INCLUDE[d365fin](includes/d365fin_md.md)] anmeldeten. Dieses Thema basiert auf Grundlage von Dimensionswertcodes von einem Office 365-Konto, welches Microsoft Azure Active Directory verwendet.  

Wenn Sie Ihr Abonnement von [!INCLUDE[d365fin](includes/d365fin_md.md)] nicht mehr aktiviert haben die Evaluationsunternehmung nicht mehr verwenden, haben Sie einen Azure Active Directory Tenant. Der Administrator oder [!INCLUDE[d365fin](includes/d365fin_md.md)] Partner verwaltet diesen Tenant in [Azure Portal](https://portal.azure.com). Dieses ist, woher neue Benutzer hinzugefügt werden und Lizenzen angewendet und entfernt werden. Weitere Informationen finden Sie unter [Microsoft Azure-Portalübersicht](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

Einer der Lizenztypen für [!INCLUDE[d365fin](includes/d365fin_md.md)] ist *Externer Buchhalter*. Dieser Lizenztyp ist für Benutzer wie externe Buchhalter gedacht. Das bedeutet, dass Sie einen zusätzlichen Arbeitsplatz in den aktuellen Active Directory nicht kaufen oder eine der vorhandenen Benutzerkonten auf [!INCLUDE[d365fin](includes/d365fin_md.md)] Ihrem externen Buchhalter verwenden müssen. Wenn beispielsweise Ihr aktuelles Office 365 Abonnement 10 Benutzer umfasst für [!INCLUDE[d365fin](includes/d365fin_md.md)] und Sie 10 *Volle Benutzer*-Lizenzen verwenden, kann der Administrator den externen Buchhalter als Gastbenutzer in Azure hinzufügen und diesem Benutzer die *Externer Buchhalter*-Lizenz ohen zusätzliche Kosten zuweisen. Sie können jedoch einen Benutzer mit der *Externer Buchhalter*-Lizenz haben. Wenn Sie mehrere Benutzer hinzufügen möchten, müssen Sie das Office 365 Abonnement entsprechend aktualisieren.  

## <a name="see-also"></a>Siehe auch
[Finanzen](finance.md)  
[Vorgehensweise: Richten Sie E-Mail Nachricht manuell oder mit der unterstützten Einrichtung ein](madeira-how-setup-email.md)  
[Buchhalter-Erfahrung in Dynamics 365 Business edition ](finance-accounting.md)  
[Dynamics 365 for Accounts in Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  
