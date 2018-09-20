Unter [powerapps.com](https://powerapps.com) können Sie anhand einer Beispiel-App Entwurfsmöglichkeiten kennen lernen. Außerdem werden Sie Konzepte entdecken, die Sie anwenden können, wenn Sie Ihre eigenen Apps entwickeln. In jeder Beispiel-App werden fiktive Daten verwendet, um ein realistisches Szenario zu veranschaulichen.

Weitere Informationen finden Sie in der Dokumentation der jeweiligen Beispiel-App.

![Beispiel-App zum Sammeln von Spenden](../media/fundraiser-app1.png)

## <a name="get-sample-apps"></a>Abrufen von Beispiel-Apps

Bevor Sie mit modellgesteuerten Beispiel-Apps experimentieren oder diese bearbeiten können, müssen Sie sie zuerst in einer Common Data Service-Datenbank einrichten. Erstellen Sie zunächst eine Testumgebung und eine Datenbank, und aktivieren Sie das Kontrollkästchen **Beispiel-Apps und -Daten einschließen**.

![Erstellen einer Datenbank](../media/create-database1.png)

> [!IMPORTANT]
> Durch Aktivierung dieses Kontrollkästchens installieren Sie alle verfügbaren Beispiel-Apps in Ihrer Datenbank. Beispiel-Apps sind für Bildungs- und Demonstrationszwecke bestimmt. Sie sollten nicht in den Produktionsdatenbanken installiert werden.

## <a name="customize-a-sample-app"></a>Anpassen einer Beispiel-App

1. Melden Sie sich bei [powerapps.com](https://powerapps.com) an, und wählen Sie **Modellgesteuert** im Entwurfsmodus aus.

    ![Auswählen des Designmodus](../media/choose-design-mode.png)

2. Zeigen Sie auf der Startseite mit der Maus auf eine Beispiel-App wie *Fundraiser*, und klicken Sie auf **Anpassen**.

    Der App-Designer wird geöffnet und bietet mehrere Optionen zum Anpassen der App an.


## <a name="remove-sample-apps-and-data"></a>Entfernen von Beispiel-Apps und -daten 
Beachten Sie folgende Punkte beim Entfernen von Beispiel-Apps und Daten:

- Löschen einer Beispiel-App erfordert das Löschen der entsprechenden [verwalteten Lösung](https://docs.microsoft.com/dynamics365/customer-engagement/developer/uninstall-delete-solution).
- Beim Löschen der Lösung werden auch ggf. für die benutzerdefinierten Entitäten spezifische Beispieldaten gelöscht.
- Wenn Anpassungen an der Beispiel-App vorgenommen wurden, liegen möglicherweise [Abhängigkeiten](https://docs.microsoft.com/dynamics365/customer-engagement/developer/dependency-tracking-solution-components) vor, die entfernt werden müssen, bevor die Lösung gelöscht werden kann.

Um Beispiel-Apps und Daten zu entfernen, gehen Sie wie folgt vor.

1. Melden Sie sich beim [Microsoft PowerApps-Verwaltungsportal](https://admin.powerapps.com) an.
2. Wählen Sie eine Umgebung aus.
3. Wählen Sie **Dynamics 365 Admin Center** aus.

    ![Dynamics 365 Admin Center](../media/admin-center.png)

4. Wählen Sie Ihre Datenbank in der Liste aus, und klicken Sie anschließend auf **Öffnen**.

    ![Auswählen einer Datenbank](../media/select-database.png)

5. Wechseln Sie zu **Einstellungen \> Lösungen**.
6. Wählen Sie die App-Lösung aus, die gelöscht werden muss, und klicken Sie anschließend **Löschen**.

    ![Löschen einer Lösung](../media/delete-solution.png)

Sie können auch zur Liste der Lösungen wechseln, indem Sie **Erweitert** im Erstellerportal auswählen und dann alle auf **.dynamics.com/** folgenden Elemente in der URL löschen.

> [!IMPORTANT]
> Löschen Sie keine anderen Systemlösungen, solange Sie die Auswirkungen nicht kennen.

## <a name="install-or-uninstall-sample-data"></a>Installieren oder Deinstallieren der Beispieldaten
1. Melden Sie sich beim [PowerApps-Verwaltungsportal](https://admin.powerapps.com) an.
1. Wählen Sie eine Umgebung aus.
1. Wählen Sie **Dynamics 365 Admin Center** aus.

    ![Dynamics 365 Admin Center](../media/admin-center.png)

1. Wählen Sie Ihre Datenbank in der Liste aus, und klicken Sie anschließend auf **Öffnen**.

    ![Auswählen einer Datenbank](../media/select-database.png)

1. Wechseln Sie zu **Einstellungen \> Datenverwaltung \> Beispieldaten**.
1. Wenn Beispieldaten installiert sind, ist die Option zum Entfernen verfügbar. Andernfalls steht die Option zum Installieren von Beispieldaten zur Verfügung.

    ![Entfernen von Beispieldaten](../media/remove-sample-data.png)
