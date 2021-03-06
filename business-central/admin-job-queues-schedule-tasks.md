---
title: Projekte für die automatische Ausführung planen
description: Geplante Aufgaben sind von der Aufgabenwarteschlange verwaltet. Diese Projektausführungsberichte und Codeunits. Die Projekte können entweder einmalig oder wiederholt ausgeführt werden.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 01/12/2021
ms.author: edupont
ms.openlocfilehash: 29b5b3f633b0fd9fcac648f0bf7149b87ae0b20d
ms.sourcegitcommit: 311e86d6abb9b59a5483324d8bb4cd1be7949248
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 01/15/2021
ms.locfileid: "5013963"
---
# <a name="use-job-queues-to-schedule-tasks"></a>Verwenden von Aufgabenwarteschlangen für die Aufgabenplanung

Die Aufgabenwarteschlangen in [!INCLUDE[prod_short](includes/prod_short.md)] ermöglichen es Benutzern, bestimmte Berichte und Codeunits zu planen und auszuführen. Die Projekte können entweder einmalig oder wiederholt ausgeführt werden. So kann es beispielsweise empfehlenswert sein, den Bericht **Verkäufer * Verkäuferstatistik** wöchentlich auszuführen, um die Verkaufserfolge eines Verkäufers zu beobachten, während die Codeunit **Genehmigungsanforderungen delegieren** täglich ausgeführt wird, um zu verhindern, dass sich Dokumente ansammeln oder anderweitig den Arbeitsablauf behindern.

Im Fenster **Projektwarteschlangeneinträge** sind alle aktuellen Aufgabenwarteschlangenposten aufgelistet. Wenn Sie eine neue Projektwarteschlange hinzufügen, die Sie planen möchten, müssen Sie die Informationen über die Art des Objekts, das Sie ausführen möchten, angeben, wie der Name und die Objekt-ID, die Sie ausführen möchten. Sie können auch Parameter hinzufügen, um das Verhalten eines Aufgabenwarteschlangenpostens festzulegen. So können Sie beispielsweise einen Parameter hinzufügen, um nur gebuchte Verkaufsaufträge zu senden. Sie benötigen die entsprechende Berechtigung zum Ausführen des jeweiligen Berichts oder der jeweiligen Codeunit, da ansonsten beim Ausführen der Projektwarteschlange ein Fehler auftritt.  
> [!IMPORTANT]  
> Wenn Sie den SUPER-Zugriffsrechtsatz der Demolizenz für [!INCLUDE[prod_short](includes/prod_short.md)] verwenden, sind Sie und Ihre Benutzer zum Ausführen aller Objekte innerhalb der Lizenz berechtigt. Dies ist immer noch nicht genug für delegierte Administratoren oder Benutzer mit Gerätelizenz, die keine Projektwarteschlangen erstellen können.

Eine Aufgabenwarteschlange kann mehrere Posten haben. Diese stellen die Projekte dar, die die Warteschlange verwaltet und ausführt. Informationen in dem Posten geben an, welche Codeunit oder welcher Bericht ausgeführt wird, wann und wie häufig der Posten ausgeführt wird, in welcher Kategorie das Projekt ausgeführt wird, und wie es ausgeführt wird.  

Nachdem Projektwarteschlangen eingerichtet sind und ausgeführt werden, kann sich der Status innerhalb jedes wiederkehrenden Zeitraums folgendermaßen ändern:

* **Abwarten**  
* **Bereit**  
* **In Bearbeitung**  
* **Fehler**  
* **Erledigt**  

Nachdem ein Projekt erfolgreich abgeschlossen wurde, wird dieses aus der Liste der Projektwarteschlangeneinträge entfernt, es sei denn, es handelt sich um ein wiederkehrendes Projekt. Wenn es sich um ein wiederkehrendes Projekt handelt, wird das Feld **Früheste Startzeit** angepasst, um anzuzeigen, wann das Projekt erwartungsgemäß das nächste Mal ausgeführt wird.  

## <a name="to-view-status-or-errors-in-the-job-queue"></a>So werden Status oder Fehler in der Projektwarteschlange angezeigt

Daten, die erstellt werden, wenn eine Projektwarteschlange ausgeführt wird, werden in der Datenbank gespeichert, sodass Sie Projektwarteschlangenfehler beheben können.  
Für jeden Projektwarteschlangeneintrag können Sie den Status anzeigen und ändern. Wenn Sie eine Projektwarteschlangenposten erstellen, wird der zugehörige Status auf **Warten** festgelegt. Sie können den Status beispielsweise auf **Bereit** und wieder auf **Warten** setzen. Andernfalls werden die Statusinformationen in diesem Feld automatisch aktualisiert.

Die folgende Tabelle beschreibt die Werte im Feld **Status**.

| Status | Beschreibung |
|--|--|
| Bereit | Gibt an, dass der Projektwarteschlangenposten ausgeführt werden kann. |
| In Bearbeitung | Gibt an, dass der Projektwarteschlangenposten in Bearbeitung ist. Dieses Feld wird aktualisiert, während die Projektwarteschlange ausgeführt wird. |
| Warten | Standard. Gibt den Status des Projektwarteschlangenpostens an, wenn dieser erstellt wird. Wählen Sie die Aktion **Status auf 'Bereit' festlegen**, um den Status auf **Bereit** zu ändern. Wählen Sie die Aktion **Auf 'Abwarten' setzen** oder **Anhalten**, um den Status wieder auf **Warten** zu ändern. |
| Fehler | Gibt an, dass ein Fehler vorliegt. Wählen Sie **Fehler anzeigen**, um die Fehlermeldung anzuzeigen. |
| Erledigt | Gibt an, dass der Projektwarteschlangenposten abgeschlossen ist. |

### <a name="to-view-status-for-any-job"></a>So wird der Status für jedes beliebige Projekt angezeigt
1. Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Tell me-Funktion") aus, geben Sie **Aufgabenwarteschlangeneinträge** ein, und wählen Sie dann den zugehörigen Link.
2. Auf der Seite **Projektwarteschlangeneinträge** wählen Sie einen Projektwarteschlangeneintrag aus, und wählen die dann die Aktion **Protokolleinträge** aus.  

> [!TIP]
> Mit [!INCLUDE [prod_short](includes/prod_short.md)] Online können Sie auch den Status von Projektwarteschlangeneinträgen mithilfe von anzeigen Application Insights in Microsoft Azure. Weitere Informationen finden Sie unter [Analysieren der Projektwarteschlange Lebenszyklus-Nachverfolgungs-Telemetrie](/dynamics365smb-devitpro\dev-itpro\administration\telemetry-job-queue-lifecycle-trace) in der [!INCLUDE [prod_short](includes/prod_short.md)] Entwickler und IT Pro Hilfe.

## <a name="the-my-job-queue-part"></a>Der „Mein Projektwarteschlangenteil”
Der Teil **Meine Projektwarteschlange** in Ihrem Rollencenter zeigt die Projektwarteschlangeneinträge an, die Sie gestartet haben, die jedoch noch nicht abgeschlossen sind. Standardmäßig ist dieser Teil nicht sichtbar, Sie müssen ihn also Ihrem Rollencenter hinzufügen. Weitere Informationen finden Sie unter [Personalisieren Sie Ihren Arbeitsbereich](ui-personalization-user.md).  

Der Teil zeigt, welche Belege mit Ihrer ID im Feld **Zugewiesene Benutzer-ID** verarbeitet oder in die Warteschlange gestellt werden, einschließlich solcher, die zur Hintergrundbuchung gehören. Dieser Teil informiert Sie auf einen Blick darüber, ob bei der Buchung eines Belegs ein Fehler aufgetreten ist, oder ob ein Projektwarteschlangenposten einen Fehler enthält. Mit diesem Teil können Sie auch eine Buchung stornieren, wenn diese nicht ausgeführt wird.

### <a name="to-view-an-error-from-the-my-job-queue-part"></a>So zeigen Sie einen Fehler aus dem Bereich Meine Projektwarteschlange an.
1. Bei einem Eintrag mit dem Status **Fehler** wählen Sie die Aktion **Fehler anzeigen** aus.
2. Überprüfen Sie die Fehlermeldung und korrigieren Sie das Problem.


## <a name="examples-of-what-can-be-scheduled-using-job-queue"></a>Beispiele dafür, was mithilfe der Projektwarteschlange geplant werden kann

### <a name="schedule-reports"></a>Berichte planen

Sie können einen Bericht oder einen Stapelverarbeitungsauftrag planen, sodass er an einem bestimmten Datum und zu einer festgelegten Uhrzeit ausgeführt wird. Geplante Berichte und Stapelverarbeitungsaufträge werden in der Projektwarteschlange eingegeben und zu der geplanten Zeit verarbeitet, wie vergleichbare andere Aufträge auch. Sie wählen die **Zeitplan** Option aus, nachdem Sie die Schaltfläche **Senden an** gewählt haben und geben Sie dann Informationen wie den Drucker sowie Uhrzeit und Datum und Serienmuster ein.  

Weitere Informationen finden Sie unter [Bericht für die Ausführung planen](ui-work-report.md#ScheduleReport)

### <a name="schedule-synchronization-between-prod_short-and-prod_short"></a>Die Synchronisierung planen zwischen [!INCLUDE[prod_short](includes/prod_short.md)] und [!INCLUDE[prod_short](includes/cds_long_md.md)]

Wenn Sie [!INCLUDE[prod_short](includes/prod_short.md)] in [!INCLUDE[prod_short](includes/cds_long_md.md)] integriert haben, können Sie die Projektwarteschlange verwenden, um zu planen, wann Sie Daten für die Datensätze synchronisieren möchten, die Sie in den beiden Geschäftsanwendungen gekoppelt haben. Abhängig von der Richtung und den Regeln, die Sie für die Integration definiert haben, können die Synchronisationsaufträge auch neue Datensätze in der Ziel-App erstellen, die denen in der Quelle entsprechen. Zum Beispiel, wenn ein Verkäufer einen neuen Kontakt in [!INCLUDE[crm_md](includes/crm_md.md)] erstellt, kann der Synchronisierungsauftrag diesen Kontakt für den gekoppelten Verkäufer in [!INCLUDE[prod_short](includes/prod_short.md)] erstellen. Weitere Informationen finden Sie unter [Planen einer Synchronisierung zwischen Business Central und Dynamics 365 Sales](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md).

### <a name="schedule-the-posting-of-sales-and-purchase-orders"></a>Planen Sie die Buchung von Verkaufsaufträgen und Einkaufsbestellungen

Projektwarteschlangen sind ein effektives Werkzeug, um die Ausführung von Geschäftsprozessen im Hintergrund zu planen, z. B. wenn mehrere Benutzer versuchen, Verkaufsaufträge zu buchen, aber nur ein Auftrag gleichzeitig verarbeitet werden kann.  

Weitere Informationen finden Sie unter [Hintergrund-Buchung mit Aufgabenwarteschlangen](ui-batch-posting.md#to-set-up-background-posting-with-job-queues)

## <a name="see-also"></a>Siehe auch

[Verwaltung](admin-setup-and-administration.md)  
[Einrichten von Business Central](setup.md)  
[Ändern von grundlegenden Einstellungen](ui-change-basic-settings.md)  
[Analysieren der Projektwarteschlangen-Lebenszyklus-Nachverfolgungs-Telemetrie](/dynamics365smb-devitpro\dev-itpro\administration\telemetry-job-queue-lifecycle-trace)  


[!INCLUDE[footer-include](includes/footer-banner.md)]