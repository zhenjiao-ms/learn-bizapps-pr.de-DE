Mit Common Data Service für Apps können Sie Daten, die von Geschäftsanwendungen verwendet werden, sicher speichern und verwalten. 

## <a name="entities"></a>Entitäten
Daten werden in Common Data Service für Apps in einer Gruppe von Datensätzen gespeichert, die als Entitäten bezeichnet werden. Eine **Entität** ist eine Gruppe von Datensätzen zum Speichern von Daten vergleichbar mit der Speicherung der Daten einer Tabelle in einer Datenbank.

Common Data Service für Apps enthält eine Basisgruppe von Standardentitäten, die gängige Geschäftsszenarien unterstützen, die sich mit Microsoft Dynamics 365-Anwendungsdaten verbinden. Sie können auch benutzerdefinierte Entitäten erstellen, die spezifisch für Ihre Organisation gelten, und diese mit Daten füllen, die Sie aus Listen in SharePoint, aus Excel oder aus Power Query importieren. App-Ersteller können dann PowerApps nutzen, um mit diesen Daten funktionsreiche Anwendungen zu entwickeln.

![Abbildung mit einer Übersicht über die Geschäftsanwendungsplattform](../media/platform.png)

Für Dynamics 365-Anwendungen, z.B. Dynamics 365 for Sales, Service und Talent, wird Common Data Service für Apps ebenfalls verwendet, um die von den Anwendungen verwendeten Daten zu speichern und zu schützen. Dies bedeutet Folgendes: Sie können Apps mit PowerApps und Common Data Service für Apps direkt basierend auf Ihren Kerngeschäftsdaten erstellen, die in Dynamics 365 bereits verwendet werden, ohne eine manuelle Integration durchführen zu müssen.

    > [!NOTE]
    > Dynamics 365 for Finance and Operations and Dynamics 365 for Retail currently require the configuration of the Data Integrator to make your business data available within Common Data Service for Apps.

![Screenshot einer Liste mit Entitäten](../media/entitylist.png "Liste mit Entitäten")

Für die meisten Organisationen ist es sinnvoll, die Standardentitäten und -attribute so wie vorgesehen zu verwenden. Sie können aber zum Erfüllen Ihrer Geschäftsanforderungen die Funktionalität von Standardentitäten erweitern, indem Sie eine oder mehrere benutzerdefinierte Entitäten zum Speichern von Informationen erstellen, die für Ihre Organisation besonders sind. 

## <a name="logic-and-validation"></a>Logik und Überprüfung
Für Entitäten in Common Data Service für Apps können die umfassenden serverseitigen Logik- und Überprüfungsfunktionen genutzt werden, um die Datenqualität sicherzustellen. Sie können auch den sich wiederholenden Code in den einzelnen Apps verringern, mit dem Daten in einer Entität erstellt und verwendet werden.

* **Geschäftsregeln**: Geschäftsregeln überprüfen Daten in mehreren Feldern und Entitäten und stellen Warn- und Fehlermeldungen bereit – unabhängig von der App, die zum Erstellen der Daten verwendet wird. 
* **Geschäftsprozessflows**: Diese Flows dienen als Anleitung für Benutzer, um sicherzustellen, dass sie Daten einheitlich eingeben und jedes Mal die gleichen Schritte ausführen. Geschäftsprozessflows werden derzeit nur für modellgesteuerte Apps unterstützt.
* **Workflows**: Workflows automatisieren Geschäftsprozesse ohne Benutzerinteraktion. 
* **Geschäftslogik mit Code**: Die Geschäftslogik unterstützt erweiterte Entwicklerszenarien, mit denen die Anwendung direkt per Code erweitert wird. 

## <a name="security"></a>Sicherheit
Daten in Common Data Service für Apps werden sicher gespeichert, sodass Benutzer sie nur anzeigen können, wenn Sie ihnen Zugriff gewähren. Bei der auf dem Dynamics 365-System basierenden rollenbasierten Sicherheit können Sie den Zugriff auf Entitäten für unterschiedliche Benutzer in Ihrer Organisation steuern.
