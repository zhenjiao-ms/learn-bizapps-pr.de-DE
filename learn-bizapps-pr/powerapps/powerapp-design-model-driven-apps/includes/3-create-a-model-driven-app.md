In dieser Einheit erstellen Sie eine modellgesteuerte App mithilfe einer der Standardentitäten, die in Ihrer Microsoft PowerApps-Umgebung verfügbar sind.

## <a name="create-your-model-driven-app"></a>Erstellen Ihrer modellgesteuerten App

1. Melden Sie sich mit Ihrem Unternehmenskonto bei [PowerApps](https://web.powerapps.com/) an.
1. Wählen Sie die gewünschte Umgebung aus, oder wechseln Sie zum [PowerApps Admin Center](https://admin.powerapps.com/), um eine neue zu erstellen.
1. Wählen Sie unten im linken Bereich **Modellgesteuert** als Entwurfsmodus aus. 

    ![Modellgesteuert](../media/choose-design-mode.png)

    > [!IMPORTANT]
    > Wenn der Entwurfsmodus **Modellgesteuert** nicht verfügbar ist, müssen Sie möglicherweise [eine Umgebung erstellen](https://docs.microsoft.com/powerapps/administrator/create-environment).

1. Wählen Sie im linken Bereich **Apps** und dann **App erstellen** aus.
1. Geben Sie auf der Seite **Neue App erstellen** einen Namen und eine Beschreibung für die App ein.
1. Wählen Sie **Fertig**aus. Ihre neue App wird im App-Designer angezeigt, und Sie können ihr nun Komponenten hinzufügen.

## <a name="add-components-to-your-app"></a>Hinzufügen von Komponenten zu Ihrer App
Sie fügen Ihrer App mit dem App-Designer Komponenten hinzu.

1. Wählen Sie den Pfeil **Designer für die Siteübersicht öffnen** aus, um den Designer für die Siteübersicht zu öffnen. 

    ![Erstellen einer neuen Siteübersicht](../media/new-sitemap.png)

2. Wählen Sie im Designer für die Siteübersicht **Neuer Unterbereich** und dann im rechten Bereich auf der Registerkarte **Eigenschaften** die folgenden Eigenschaften aus:

    - **Typ**: Entität
    - **Entität**: Konto

    ![Hinzufügen von Komponenten zur Siteübersicht](../media/sitemap.png)

3. Wählen Sie **Speichern und Schließen** aus.
4. Wählen Sie im App-Designer **Formulare** und dann im rechten Bereich unter **Hauptformulare** das Formular **Konto** aus.

    ![Kontohauptformular](../media/main-form.png)

5. Wählen Sie im App-Designer **Ansichten** und dann die folgenden Eigenschaften aus:

    - Aktive Konten
    - Alle Konten
    - Meine aktiven Konten

6. Wählen Sie im App-Designer **Diagramme** und dann das Diagramm **Firmen nach Branche** aus.
7. Wählen Sie auf der App-Designer-Symbolleiste **Speichern** aus.

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