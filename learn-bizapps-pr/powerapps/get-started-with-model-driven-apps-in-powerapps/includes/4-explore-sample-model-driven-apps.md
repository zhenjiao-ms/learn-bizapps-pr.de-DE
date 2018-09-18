<span data-ttu-id="5e224-101">Unter [powerapps.com](https://powerapps.com) können Sie anhand einer Beispiel-App Entwurfsmöglichkeiten kennen lernen.</span><span class="sxs-lookup"><span data-stu-id="5e224-101">On [powerapps.com](https://powerapps.com), you can use a sample app to explore design possibilities.</span></span> <span data-ttu-id="5e224-102">Außerdem werden Sie Konzepte entdecken, die Sie anwenden können, wenn Sie Ihre eigenen Apps entwickeln.</span><span class="sxs-lookup"><span data-stu-id="5e224-102">You'll also discover concepts that you can apply as you develop your own apps.</span></span> <span data-ttu-id="5e224-103">In jeder Beispiel-App werden fiktive Daten verwendet, um ein realistisches Szenario zu veranschaulichen.</span><span class="sxs-lookup"><span data-stu-id="5e224-103">Every sample app uses fictitious data to showcase a real-world scenario.</span></span>

<span data-ttu-id="5e224-104">Weitere Informationen finden Sie in der Dokumentation der jeweiligen Beispiel-App.</span><span class="sxs-lookup"><span data-stu-id="5e224-104">For more details, be sure to check out the documentation that's specific to each sample app.</span></span>

![Beispiel-App zum Sammeln von Spenden](../media/fundraiser-app1.png)

## <a name="get-sample-apps"></a><span data-ttu-id="5e224-106">Abrufen von Beispiel-Apps</span><span class="sxs-lookup"><span data-stu-id="5e224-106">Get sample apps</span></span>

<span data-ttu-id="5e224-107">Bevor Sie mit modellgesteuerten Beispiel-Apps experimentieren oder diese bearbeiten können, müssen Sie sie zuerst in einer Common Data Service-Datenbank einrichten.</span><span class="sxs-lookup"><span data-stu-id="5e224-107">Before you can play around with or edit the model-driven sample apps, you must set them up in a Common Data Service database.</span></span> <span data-ttu-id="5e224-108">Erstellen Sie zunächst eine Testumgebung und eine Datenbank, und aktivieren Sie das Kontrollkästchen **Beispiel-Apps und -Daten einschließen**.</span><span class="sxs-lookup"><span data-stu-id="5e224-108">First, create a trial environment and database, and be sure to select the **Include sample apps and data** check box.</span></span>

![Erstellen einer Datenbank](../media/create-database1.png)

> [!IMPORTANT]
> <span data-ttu-id="5e224-110">Durch Aktivierung dieses Kontrollkästchens installieren Sie alle verfügbaren Beispiel-Apps in Ihrer Datenbank.</span><span class="sxs-lookup"><span data-stu-id="5e224-110">By selecting this check box, you install all available sample apps in your database.</span></span> <span data-ttu-id="5e224-111">Beispiel-Apps sind für Bildungs- und Demonstrationszwecke bestimmt.</span><span class="sxs-lookup"><span data-stu-id="5e224-111">Sample apps are for educational and demonstration purposes.</span></span> <span data-ttu-id="5e224-112">Sie sollten nicht in den Produktionsdatenbanken installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5e224-112">We don't recommend installing them in production databases.</span></span>

## <a name="customize-a-sample-app"></a><span data-ttu-id="5e224-113">Anpassen einer Beispiel-App</span><span class="sxs-lookup"><span data-stu-id="5e224-113">Customize a sample app</span></span>

1. <span data-ttu-id="5e224-114">Melden Sie sich bei [powerapps.com](https://powerapps.com) an, und wählen Sie **Modellgesteuert** im Entwurfsmodus aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-114">Sign in to [powerapps.com](https://powerapps.com), and select **Model-driven** as the design mode.</span></span>

    ![Auswählen des Entwurfsmodus](../media/choose-design-mode.png)

2. <span data-ttu-id="5e224-116">Bewegen Sie den Mauszeiger auf der Startseite über eine Beispiel-App, und wählen Sie **Anpassen** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-116">On the home page, hover over a sample app, and select **Customize**.</span></span>

    <span data-ttu-id="5e224-117">Der App-Designer wird geöffnet und bietet mehrere Optionen zum Anpassen der App an.</span><span class="sxs-lookup"><span data-stu-id="5e224-117">The App Designer opens, providing multiple options for customizing the app.</span></span>

3. <span data-ttu-id="5e224-118">Wählen Sie zur Anzeige weiterer Anpassungsoptionen im linken Bereich **Erweitert** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-118">For more customization options, select **Advanced** in the left pane.</span></span>

## <a name="remove-sample-apps-and-data"></a><span data-ttu-id="5e224-119">Entfernen von Beispiel-Apps und Daten</span><span class="sxs-lookup"><span data-stu-id="5e224-119">Remove sample apps and data</span></span> 
<span data-ttu-id="5e224-120">Beachten Sie folgende Punkte beim Entfernen von Beispiel-Apps und Daten:</span><span class="sxs-lookup"><span data-stu-id="5e224-120">Keep these points in mind when removing samples apps and data:</span></span>

- <span data-ttu-id="5e224-121">Löschen einer Beispiel-App erfordert das Löschen der entsprechenden [verwalteten Lösung](https://docs.microsoft.com/dynamics365/customer-engagement/developer/uninstall-delete-solution).</span><span class="sxs-lookup"><span data-stu-id="5e224-121">Deleting a sample app requires deleting the corresponding [managed solution](https://docs.microsoft.com/dynamics365/customer-engagement/developer/uninstall-delete-solution).</span></span>
- <span data-ttu-id="5e224-122">Beim Löschen der Lösung werden auch ggf. für die benutzerdefinierten Entitäten spezifische Beispieldaten gelöscht.</span><span class="sxs-lookup"><span data-stu-id="5e224-122">Deleting the solution also deletes any sample data that's specific to the custom entities for the app.</span></span>
- <span data-ttu-id="5e224-123">Wenn Anpassungen an der Beispiel-App vorgenommen wurden, liegen möglicherweise [Abhängigkeiten](https://docs.microsoft.com/dynamics365/customer-engagement/developer/dependency-tracking-solution-components) vor, die entfernt werden müssen, bevor die Lösung gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="5e224-123">If customizations were made to the sample app, there might be [dependencies](https://docs.microsoft.com/dynamics365/customer-engagement/developer/dependency-tracking-solution-components) that must be removed before the solution can be deleted.</span></span>

<span data-ttu-id="5e224-124">Um Beispiel-Apps und Daten zu entfernen, gehen Sie wie folgt vor.</span><span class="sxs-lookup"><span data-stu-id="5e224-124">To remove sample apps and data, follow these steps.</span></span>

1. <span data-ttu-id="5e224-125">Melden Sie sich beim [Microsoft PowerApps-Verwaltungsportal](https://admin.powerapps.com) an.</span><span class="sxs-lookup"><span data-stu-id="5e224-125">Sign in to the [Microsoft PowerApps admin portal](https://admin.powerapps.com).</span></span>
2. <span data-ttu-id="5e224-126">Wählen Sie eine Umgebung aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-126">Select an environment.</span></span>
3. <span data-ttu-id="5e224-127">Wählen Sie **Dynamics 365 Admin Center** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-127">Select **Dynamics 365 Administration Center**.</span></span>

    ![Dynamics 365 Administration Center](../media/admin-center.png)

4. <span data-ttu-id="5e224-129">Wählen Sie die Datenbank in der Liste und dann **Öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-129">Select your database in the list, and then select **Open**.</span></span>

    ![Auswählen einer Datenbank](../media/select-database.png)

5. <span data-ttu-id="5e224-131">Wechseln Sie zu **Einstellungen \> Lösungen**.</span><span class="sxs-lookup"><span data-stu-id="5e224-131">Go to **Settings \> Solutions**.</span></span>
6. <span data-ttu-id="5e224-132">Wählen Sie die Lösung für die App, die gelöscht werden muss, und dann **Löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-132">Select the solution for the app that must be deleted, and then select **Delete**.</span></span>

    ![Löschen einer Lösung](../media/delete-solution.png)

<span data-ttu-id="5e224-134">Sie können auch zur Liste der Lösungen wechseln, indem Sie **Erweitert** im Erstellerportal auswählen und dann alle auf **.dynamics.com/** folgenden Elemente in der URL löschen.</span><span class="sxs-lookup"><span data-stu-id="5e224-134">You can also go to the list of solutions by selecting **Advanced** in the maker portal and then deleting everything in the URL after **.dynamics.com/**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e224-135">Löschen Sie keine anderen Systemlösungen, solange Sie die Auswirkungen nicht kennen.</span><span class="sxs-lookup"><span data-stu-id="5e224-135">Don't delete other system solutions unless you're aware of the effect.</span></span>

## <a name="install-or-uninstall-sample-data"></a><span data-ttu-id="5e224-136">Installieren oder Deinstallieren der Beispieldaten</span><span class="sxs-lookup"><span data-stu-id="5e224-136">Install or uninstall sample data</span></span>
1. <span data-ttu-id="5e224-137">Melden Sie sich beim [PowerApps-Verwaltungsportal](https://admin.powerapps.com) an.</span><span class="sxs-lookup"><span data-stu-id="5e224-137">Sign in to the [PowerApps admin portal](https://admin.powerapps.com).</span></span>
1. <span data-ttu-id="5e224-138">Wählen Sie eine Umgebung aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-138">Select an environment.</span></span>
1. <span data-ttu-id="5e224-139">Wählen Sie **Dynamics 365 Admin Center** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-139">Select **Dynamics 365 Administration Center**.</span></span>

    ![Dynamics 365 Administration Center](../media/admin-center.png)

1. <span data-ttu-id="5e224-141">Wählen Sie die Datenbank in der Liste und dann **Öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="5e224-141">Select your database in the list, and then select **Open**.</span></span>

    ![Auswählen einer Datenbank](../media/select-database.png)

1. <span data-ttu-id="5e224-143">Wechseln Sie zu **Einstellungen \> Datenverwaltung \> Beispieldaten**.</span><span class="sxs-lookup"><span data-stu-id="5e224-143">Go to **Settings \> Data Management \> Sample Data**.</span></span>
1. <span data-ttu-id="5e224-144">Wenn Beispieldaten installiert sind, ist die Option zum Entfernen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5e224-144">If sample data is installed, the option to remove it is available.</span></span> <span data-ttu-id="5e224-145">Andernfalls steht die Option zum Installieren von Beispieldaten zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="5e224-145">Otherwise, the option to install sample data is available.</span></span>

    ![Entfernen von Beispieldaten](../media/remove-sample-data.png)
