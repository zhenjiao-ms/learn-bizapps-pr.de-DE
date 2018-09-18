<span data-ttu-id="6db85-101">In dieser Einheit erstellen Sie eine modellgesteuerte App mithilfe einer der Standardentitäten, die in Ihrer Microsoft PowerApps-Umgebung verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="6db85-101">In this unit, you'll create a model-driven app by using one of the standard entities that's available in your Microsoft PowerApps environment.</span></span>

## <a name="create-a-model-driven-app"></a><span data-ttu-id="6db85-102">Erstellen einer modellgesteuerten App</span><span class="sxs-lookup"><span data-stu-id="6db85-102">Create a model-driven app</span></span>

1. <span data-ttu-id="6db85-103">Melden Sie sich mit Ihrem Unternehmenskonto bei [PowerApps](https://web.powerapps.com/) an.</span><span class="sxs-lookup"><span data-stu-id="6db85-103">Sign in to [PowerApps](https://web.powerapps.com/) by using your organizational account.</span></span>
1. <span data-ttu-id="6db85-104">Wählen Sie die gewünschte Umgebung aus, oder wechseln Sie zum [PowerApps Admin Center](https://admin.powerapps.com/), um eine neue zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6db85-104">Select the environment you want, or go to the [PowerApps admin center](https://admin.powerapps.com/) to create a new one.</span></span>
1. <span data-ttu-id="6db85-105">Wählen Sie unten im linken Bereich **Modellgesteuert** als Entwurfsmodus aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-105">At the bottom of the left pane, select **Model-driven** as the design mode.</span></span> 

    ![Modellgesteuert](../media/choose-design-mode.png)

    > [!IMPORTANT]
    > <span data-ttu-id="6db85-107">Wenn der Entwurfsmodus **Modellgesteuert** nicht verfügbar ist, müssen Sie möglicherweise [eine Umgebung erstellen](https://docs.microsoft.com/powerapps/administrator/create-environment).</span><span class="sxs-lookup"><span data-stu-id="6db85-107">If the **Model-driven** design mode isn't available, you might need to [create an environment](https://docs.microsoft.com/powerapps/administrator/create-environment).</span></span>

1. <span data-ttu-id="6db85-108">Wählen Sie im linken Bereich **Apps** und dann **App erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-108">In the left pane, select **Apps**, and then select **Create an app**.</span></span>
1. <span data-ttu-id="6db85-109">Geben Sie auf der Seite **Neue App erstellen** einen Namen und eine Beschreibung für die App ein.</span><span class="sxs-lookup"><span data-stu-id="6db85-109">On the **Create a New App** page, enter a name and description for the app.</span></span>
1. <span data-ttu-id="6db85-110">Wählen Sie **Fertig**aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-110">Select **Done**.</span></span> <span data-ttu-id="6db85-111">Ihre neue App wird im App-Designer angezeigt, und Sie können ihr nun Komponenten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6db85-111">Your new app appears in the App Designer, and you can now add components to it.</span></span>

## <a name="add-components-to-your-app"></a><span data-ttu-id="6db85-112">Hinzufügen von Komponenten zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="6db85-112">Add components to your app</span></span>
<span data-ttu-id="6db85-113">Sie fügen Ihrer App mit dem App-Designer Komponenten hinzu.</span><span class="sxs-lookup"><span data-stu-id="6db85-113">You add components to your app by using the App Designer.</span></span>

1. <span data-ttu-id="6db85-114">Wählen Sie den Pfeil **Designer für die Siteübersicht öffnen** aus, um den Designer für die Siteübersicht zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="6db85-114">Select the **Open the Site Map Designer** arrow to open the site map designer.</span></span>

    ![Erstellen einer neuen Siteübersicht](../media/new-sitemap.png)

2. <span data-ttu-id="6db85-116">Wählen Sie im Designer für die Siteübersicht **Neuer Unterbereich** und dann im rechten Bereich auf der Registerkarte **Eigenschaften** die folgenden Eigenschaften aus:</span><span class="sxs-lookup"><span data-stu-id="6db85-116">In the site map designer, select **New Subarea**, and then, in the right pane, on the **Properties** tab, select the following properties:</span></span>

    - <span data-ttu-id="6db85-117">**Typ**: *Entität*</span><span class="sxs-lookup"><span data-stu-id="6db85-117">**Type**: *Entity*</span></span>
    - <span data-ttu-id="6db85-118">**Entität**: *Konto*</span><span class="sxs-lookup"><span data-stu-id="6db85-118">**Entity**: *Account*</span></span>

    ![Hinzufügen von Komponenten zur Siteübersicht](../media/sitemap.png)

3. <span data-ttu-id="6db85-120">Wählen Sie **Speichern und Schließen** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-120">Select **Save And Close**.</span></span>
4. <span data-ttu-id="6db85-121">Wählen Sie im App-Designer **Formulare** und dann im rechten Bereich unter **Hauptformulare** das Formular **Konto** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-121">In the App Designer, select **Forms**, and then, in the right pane, under **Main Forms**, select the **Account** form.</span></span>

    ![Kontohauptformular](../media/main-form.png)

5. <span data-ttu-id="6db85-123">Wählen Sie im App-Designer **Ansichten** und dann die folgenden Eigenschaften aus:</span><span class="sxs-lookup"><span data-stu-id="6db85-123">In the App Designer, select **Views**, and then select the following properties:</span></span>

    - <span data-ttu-id="6db85-124">Aktive Konten</span><span class="sxs-lookup"><span data-stu-id="6db85-124">Active Accounts</span></span>
    - <span data-ttu-id="6db85-125">Alle Konten</span><span class="sxs-lookup"><span data-stu-id="6db85-125">All Accounts</span></span>
    - <span data-ttu-id="6db85-126">Meine aktiven Konten</span><span class="sxs-lookup"><span data-stu-id="6db85-126">My Active Accounts</span></span>

6. <span data-ttu-id="6db85-127">Wählen Sie im App-Designer **Diagramme** und dann das Diagramm **Firmen nach Branche** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-127">In the App Designer, select **Charts**, and then select the **Accounts by Industry** chart.</span></span>
7. <span data-ttu-id="6db85-128">Wählen Sie auf der App-Designer-Symbolleiste **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-128">On the App Designer toolbar, select **Save**.</span></span>

<!-- ##  Validate your app
This step checks for component dependencies that are required for the app to work, but haven't yet been added to the app. 

1. On the app designer canvas, select the component that indicates a dependency, such as the **Forms** component. Then, on the right-pane select the **Required** tab, expand **Entity Dependencies** and then select all required dependencies. 

    ![Add dependencies](../media/build-first-model-driven-app/resolve-dependencies.png)

2. Select **Add Dependencies**.
3. On the app designer toolbar, select **Save**.  -->

## <a name="publish-your-app"></a><span data-ttu-id="6db85-129">Veröffentlichen der App</span><span class="sxs-lookup"><span data-stu-id="6db85-129">Publish your app</span></span>
<span data-ttu-id="6db85-130">Wählen Sie auf der App-Designer-Symbolleiste **Veröffentlichen** aus.</span><span class="sxs-lookup"><span data-stu-id="6db85-130">On the App Designer toolbar, select **Publish**.</span></span>

<span data-ttu-id="6db85-131">Nachdem Sie die App veröffentlicht haben, können Sie sie ausführen oder für andere Benutzer freigeben.</span><span class="sxs-lookup"><span data-stu-id="6db85-131">After you publish the app, it's ready for you to run or share with others.</span></span>

![Einfache Kontoentitäts-App](../media/accounts-quickstart-app.png)
