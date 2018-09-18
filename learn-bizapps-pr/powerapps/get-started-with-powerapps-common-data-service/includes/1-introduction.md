Mit dem Common Data Service (CDS) für Apps können Sie Daten, die von Geschäftsanwendungen verwendet werden, sicher speichern und verwalten. 

## <a name="entities"></a>Entitäten
In CDS für Apps werden Daten in einer Gruppe von Datensätzen gespeichert, die als Entitäten bezeichnet werden. Eine *Entität* ist eine Gruppe von Datensätzen zum Speichern von Daten vergleichbar mit der Speicherung von Daten einer Tabelle in einer Datenbank.

CDS für Apps enthält eine Basisgruppe von Standardentitäten, die gängige Geschäftsszenarien unterstützen, die sich mit Microsoft Dynamics 365 Anwendungsdaten verbinden. Sie können auch benutzerdefinierte Entitäten erstellen, die spezifisch für Ihre Organisation sind, und diese mit Daten füllen, die Sie aus Microsoft SharePoint-Listen, Microsoft Excel oder Microsoft Power Query für Excel importieren. App-Ersteller können dann PowerApps nutzen, um mit diesen Daten anspruchsvolle Anwendungen zu entwickeln.

![Abbildung mit einer Übersicht über die Geschäftsanwendungsplattform](../media/platform.png)

Dynamics 365-Anwendungen, einschließlich Dynamics 365 for Sales, Dynamics 365 for Service und Dynamics 365 for Talent, verwenden CDS für Apps zum Speichern und Schützen der von ihnen verwendeten Daten. Das bedeutet, dass Sie mit PowerApps und CDS für Apps Anwendungen direkt anhand wichtiger Geschäftsdaten erstellen können, die bereits in Dynamics 365 verwendet werden, ohne dass eine manuelle Integration erforderlich ist.

> [!NOTE]
> Dynamics 365 for Finance and Operations und Dynamics 365 for Retail erfordern derzeit die Einrichtung des Datenintegrators, um Ihre Geschäftsdaten in CDS für Apps verfügbar zu machen.

![Screenshot einer Liste mit Entitäten](../media/entitylist.png "Liste mit Entitäten")

Für die meisten Organisationen ist es sinnvoll, die Standardentitäten und -attribute so wie vorgesehen zu verwenden. Sie können aber zum Erfüllen Ihrer Geschäftsanforderungen die Funktionalität von Standardentitäten erweitern, indem Sie eine oder mehrere benutzerdefinierte Entitäten zum Speichern von Informationen erstellen, die für Ihre Organisation besonders sind. 

## <a name="logic-and-validation"></a>Logik und Überprüfung
Entitäten in CDS für Apps können die umfassenden serverseitigen Logik- und Überprüfungsfunktionen nutzen, um Datenqualität sicherzustellen. Sie können auch den sich wiederholenden Code in den einzelnen Apps verringern, mit dem Daten in einer Entität erstellt und verwendet werden.

* **Geschäftsregeln**: Geschäftsregeln überprüfen Daten in mehreren Feldern und Entitäten und stellen Warn- und Fehlermeldungen bereit – unabhängig von der App, die zum Erstellen der Daten verwendet wird. 
* **Geschäftsprozessflows**: Diese Flows dienen als Anleitung für Benutzer, um sicherzustellen, dass sie Daten einheitlich eingeben und jedes Mal die gleichen Schritte ausführen. Geschäftsprozessflows werden derzeit nur für modellgesteuerte Apps unterstützt.
* **Workflows**: Workflows automatisieren Geschäftsprozesse ohne Benutzerinteraktion. 
* **Geschäftslogik mit Code**: Die Geschäftslogik unterstützt erweiterte Entwicklerszenarien, mit denen die Anwendung direkt per Code erweitert wird. 

## <a name="security"></a>Sicherheit
Daten in CDS für Apps werden sicher gespeichert, sodass Benutzer sie nur anzeigen können, wenn Sie ihnen Zugriff gewähren. Bei der auf dem Dynamics 365-System basierenden rollenbasierten Sicherheit können Sie den Zugriff auf Entitäten für unterschiedliche Benutzer in Ihrer Organisation steuern.