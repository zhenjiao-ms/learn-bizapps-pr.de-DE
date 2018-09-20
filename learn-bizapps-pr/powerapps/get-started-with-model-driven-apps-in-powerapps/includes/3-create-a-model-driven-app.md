<span data-ttu-id="ee323-101">In dieser Einheit erfahren Sie, wie Sie eine modellgesteuerte App mithilfe einer der Standardentitäten erstellen, die in Ihrer Microsoft PowerApps-Umgebung verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="ee323-101">In this unit, you'll create a model-driven app by using one of the standard entities that's available in your Microsoft PowerApps environment.</span></span>

## <a name="create-a-model-driven-app"></a><span data-ttu-id="ee323-102">Erstellen einer modellgesteuerten App</span><span class="sxs-lookup"><span data-stu-id="ee323-102">Create a model-driven app</span></span>

1. <span data-ttu-id="ee323-103">Melden Sie sich mit Ihrem Unternehmenskonto bei [PowerApps](https://web.powerapps.com/) an.</span><span class="sxs-lookup"><span data-stu-id="ee323-103">Sign in to [PowerApps](https://web.powerapps.com/) by using your organizational account.</span></span>
1. <span data-ttu-id="ee323-104">Wählen Sie die gewünschte Umgebung aus, oder wechseln Sie zum [PowerApps Admin Center](https://admin.powerapps.com/), um eine neue zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ee323-104">Select the environment you want, or go to the [PowerApps admin center](https://admin.powerapps.com/) to create a new one.</span></span>
1. <span data-ttu-id="ee323-105">Wählen Sie unten im linken Bereich **Modellgesteuert** als Entwurfsmodus aus.</span><span class="sxs-lookup"><span data-stu-id="ee323-105">At the bottom of the left pane, select **Model-driven** as the design mode.</span></span> 

    ![Modellgesteuert](../media/choose-design-mode.png)

    > [!IMPORTANT]
    > <span data-ttu-id="ee323-107">Wenn der Entwurfsmodus **Modellgesteuert** nicht verfügbar ist, müssen Sie möglicherweise [eine Umgebung erstellen](https://docs.microsoft.com/powerapps/administrator/create-environment).</span><span class="sxs-lookup"><span data-stu-id="ee323-107">If the **Model-driven** design mode isn't available, you might need to [create an environment](https://docs.microsoft.com/powerapps/administrator/create-environment).</span></span>

1. <span data-ttu-id="ee323-108">Klicken Sie im linken Bereich auf **Apps** und anschließend auf **App erstellen**.</span><span class="sxs-lookup"><span data-stu-id="ee323-108">In the left pane, select **Apps**, then select **Create an app**.</span></span>
1. <span data-ttu-id="ee323-109">Geben Sie auf der Seite **Neue App erstellen** einen Namen und eine Beschreibung für die App ein.</span><span class="sxs-lookup"><span data-stu-id="ee323-109">On the **Create a New App** page, enter a name and description for the app.</span></span>
1. <span data-ttu-id="ee323-110">Klicken Sie auf **Fertig**.</span><span class="sxs-lookup"><span data-stu-id="ee323-110">Select **Done**.</span></span> <span data-ttu-id="ee323-111">Ihre neue App wird im App-Designer angezeigt, und Sie können ihr nun Komponenten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ee323-111">Your new app appears in the App Designer, and you can now add components to it.</span></span>

## <a name="add-components-to-your-app"></a><span data-ttu-id="ee323-112">Hinzufügen von Komponenten zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="ee323-112">Add components to your app</span></span>
<span data-ttu-id="ee323-113">Sie fügen Ihrer App mit dem App-Designer Komponenten hinzu.</span><span class="sxs-lookup"><span data-stu-id="ee323-113">You add components to your app by using the App Designer.</span></span>

1. <span data-ttu-id="ee323-114">Wählen Sie den Pfeil **Designer für die Siteübersicht öffnen** aus, um den Designer für die Siteübersicht zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="ee323-114">Select the **Open the Site Map Designer** arrow to open the site map designer.</span></span>

    ![Erstellen einer neuen Siteübersicht](../media/new-sitemap.png)

2. <span data-ttu-id="ee323-116">Klicken Sie im Designer für die Siteübersicht auf **New Subarea** (Neuer Unterbereich), und wählen Sie dann im rechten Bereich auf der Registerkarte **Eigenschaften** die folgenden Eigenschaften aus:</span><span class="sxs-lookup"><span data-stu-id="ee323-116">In the site map designer, select **New Subarea**, and then, in the right pane on the **Properties** tab, select the following properties:</span></span>

    - <span data-ttu-id="ee323-117">**Typ**: *Entität*</span><span class="sxs-lookup"><span data-stu-id="ee323-117">**Type**: *Entity*</span></span>
    - <span data-ttu-id="ee323-118">**Entität**: *Konto*</span><span class="sxs-lookup"><span data-stu-id="ee323-118">**Entity**: *Account*</span></span>

    ![Hinzufügen von Komponenten zur Siteübersicht](../media/sitemap.png)

3. <span data-ttu-id="ee323-120">Klicken Sie auf **Speichern und Schließen**.</span><span class="sxs-lookup"><span data-stu-id="ee323-120">Select **Save And Close**.</span></span>
4. <span data-ttu-id="ee323-121">Klicken Sie erst im App-Designer auf **Formulare** und dann im rechten Bereich unter **Main Forms** (Hauptformulare) auf das Formular **Konto**.</span><span class="sxs-lookup"><span data-stu-id="ee323-121">In the App Designer, select **Forms**, and then, in the right pane under **Main Forms**, select the **Account** form.</span></span>

    ![Hauptformular des Kontos](../media/main-form.png)

5. <span data-ttu-id="ee323-123">Klicken Sie im App-Designer auf **Ansichten**, und wählen Sie dann die folgenden Eigenschaften aus:</span><span class="sxs-lookup"><span data-stu-id="ee323-123">In the App Designer, select **Views**, then select the following properties:</span></span>

    - <span data-ttu-id="ee323-124">Aktive Konten</span><span class="sxs-lookup"><span data-stu-id="ee323-124">Active Accounts</span></span>
    - <span data-ttu-id="ee323-125">Alle Konten</span><span class="sxs-lookup"><span data-stu-id="ee323-125">All Accounts</span></span>
    - <span data-ttu-id="ee323-126">Meine aktiven Konten</span><span class="sxs-lookup"><span data-stu-id="ee323-126">My Active Accounts</span></span>

6. <span data-ttu-id="ee323-127">Klicken Sie im App-Designer auf **Diagramme**, und wählen Sie dann das Diagramm **Accounts by Industry** (Firmen nach Branche) aus.</span><span class="sxs-lookup"><span data-stu-id="ee323-127">In the App Designer, select **Charts**, then select the **Accounts by Industry** chart.</span></span>
7. <span data-ttu-id="ee323-128">Klicken Sie auf der App-Designer-Symbolleiste auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="ee323-128">On the App Designer toolbar, select **Save**.</span></span>

<!-- ##  Validate your app
This step checks for component dependencies that are required for the app to work, but haven't yet been added to the app. 

1. On the app designer canvas, select the component that indicates a dependency, such as the **Forms** component. Then, on the right-pane select the **Required** tab, expand **Entity Dependencies** and then select all required dependencies. 

    ![Add dependencies](../media/build-first-model-driven-app/resolve-dependencies.png)

2. Select **Add Dependencies**.
3. On the app designer toolbar, select **Save**.  -->

## <a name="publish-your-app"></a><span data-ttu-id="ee323-129">Veröffentlichen der App</span><span class="sxs-lookup"><span data-stu-id="ee323-129">Publish your app</span></span>
<span data-ttu-id="ee323-130">Wählen Sie auf der App-Designer-Symbolleiste **Veröffentlichen** aus.</span><span class="sxs-lookup"><span data-stu-id="ee323-130">On the App Designer toolbar, select **Publish**.</span></span>

<span data-ttu-id="ee323-131">Nachdem Sie die App veröffentlicht haben, können Sie sie ausführen oder für andere Benutzer freigeben.</span><span class="sxs-lookup"><span data-stu-id="ee323-131">After you publish the app, it's ready for you to run or share with others.</span></span>

![Einfache Kontoentitäts-App](../media/accounts-quickstart-app.png)
