In dieser Einheit erfahren Sie, wie Sie eine modellgesteuerte App mithilfe einer der Standardentitäten erstellen, die in Ihrer Microsoft PowerApps-Umgebung verfügbar sind.

## <a name="create-a-model-driven-app"></a>Erstellen einer modellgesteuerten App

1. Melden Sie sich mit Ihrem Unternehmenskonto bei [PowerApps](https://web.powerapps.com/) an.
1. Wählen Sie die gewünschte Umgebung aus, oder wechseln Sie zum [PowerApps Admin Center](https://admin.powerapps.com/), um eine neue zu erstellen.
1. Wählen Sie unten im linken Bereich **Modellgesteuert** als Entwurfsmodus aus. 

    ![Modellgesteuert](../media/choose-design-mode.png)

    > [!IMPORTANT]
    > Wenn der Entwurfsmodus **Modellgesteuert** nicht verfügbar ist, müssen Sie möglicherweise [eine Umgebung erstellen](https://docs.microsoft.com/powerapps/administrator/create-environment).

1. Klicken Sie im linken Bereich auf **Apps** und anschließend auf **App erstellen**.
1. Geben Sie auf der Seite **Neue App erstellen** einen Namen und eine Beschreibung für die App ein.
1. Klicken Sie auf **Fertig**. Ihre neue App wird im App-Designer angezeigt, und Sie können ihr nun Komponenten hinzufügen.

## <a name="add-components-to-your-app"></a>Hinzufügen von Komponenten zu Ihrer App
Sie fügen Ihrer App mit dem App-Designer Komponenten hinzu.

1. Wählen Sie den Pfeil **Designer für die Siteübersicht öffnen** aus, um den Designer für die Siteübersicht zu öffnen.

    ![Erstellen einer neuen Siteübersicht](../media/new-sitemap.png)

2. Klicken Sie im Designer für die Siteübersicht auf **New Subarea** (Neuer Unterbereich), und wählen Sie dann im rechten Bereich auf der Registerkarte **Eigenschaften** die folgenden Eigenschaften aus:

    - **Typ**: *Entität*
    - **Entität**: *Konto*

    ![Hinzufügen von Komponenten zur Siteübersicht](../media/sitemap.png)

3. Klicken Sie auf **Speichern und Schließen**.
4. Klicken Sie erst im App-Designer auf **Formulare** und dann im rechten Bereich unter **Main Forms** (Hauptformulare) auf das Formular **Konto**.

    ![Hauptformular des Kontos](../media/main-form.png)

5. Klicken Sie im App-Designer auf **Ansichten**, und wählen Sie dann die folgenden Eigenschaften aus:

    - Aktive Konten
    - Alle Konten
    - Meine aktiven Konten

6. Klicken Sie im App-Designer auf **Diagramme**, und wählen Sie dann das Diagramm **Accounts by Industry** (Firmen nach Branche) aus.
7. Klicken Sie auf der App-Designer-Symbolleiste auf **Speichern**.

<!-- ##  Validate your app
This step checks for component dependencies that are required for the app to work, but haven't yet been added to the app. 

1. On the app designer canvas, select the component that indicates a dependency, such as the **Forms** component. Then, on the right-pane select the **Required** tab, expand **Entity Dependencies** and then select all required dependencies. 

    ![Add dependencies](../media/build-first-model-driven-app/resolve-dependencies.png)

2. Select **Add Dependencies**.
3. On the app designer toolbar, select **Save**.  -->

## <a name="publish-your-app"></a>Veröffentlichen der App
Wählen Sie auf der App-Designer-Symbolleiste **Veröffentlichen** aus.

Nachdem Sie die App veröffentlicht haben, können Sie sie ausführen oder für andere Benutzer freigeben.

![Einfache Kontoentitäts-App](../media/accounts-quickstart-app.png)
