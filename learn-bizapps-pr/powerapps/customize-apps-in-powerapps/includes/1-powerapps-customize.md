<span data-ttu-id="3228c-101">In einer vorherigen Einheit haben Sie die Flooring Estimates-App erstellt und sich mit ihrem Standarddesign vertraut gemacht.</span><span class="sxs-lookup"><span data-stu-id="3228c-101">In a previous unit, you generated the Flooring Estimates app and started to explore its default design.</span></span> <span data-ttu-id="3228c-102">Von PowerApps generierte Standard-Apps sind nützlich. Häufig müssen Sie diese jedoch an Ihre eigenen Anforderungen anpassen.</span><span class="sxs-lookup"><span data-stu-id="3228c-102">Apps that Microsoft PowerApps generates are useful out of the box, but you'll often want to customize a generated app to suit your needs.</span></span>

<span data-ttu-id="3228c-103">In dieser Einheit erläutern wir einige einfache Änderungen, die für die einzelnen App-Bildschirme vorgenommen werden können.</span><span class="sxs-lookup"><span data-stu-id="3228c-103">In this unit, we'll walk you through some basic changes for each screen in the app.</span></span> <span data-ttu-id="3228c-104">Es gibt zwar noch deutlich mehr Möglichkeiten zum Anpassen der App, doch für die ersten Schritte empfiehlt es sich, Anpassungen an einer generierten App vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="3228c-104">You can do a lot more to customize an app, but the best way to start learning is to take any generated app and make common customizations.</span></span>

## <a name="browse-screen"></a><span data-ttu-id="3228c-105">Bildschirm zum Durchsuchen</span><span class="sxs-lookup"><span data-stu-id="3228c-105">Browse screen</span></span>
<span data-ttu-id="3228c-106">Wir beginnen mit dem Bildschirm zum Durchsuchen.</span><span class="sxs-lookup"><span data-stu-id="3228c-106">We'll start on the browse screen.</span></span> <span data-ttu-id="3228c-107">In der App ist jedem Produkt bereits ein Bild und ein Text zugeordnet, doch das Layout könnte ansprechender gestaltet werden.</span><span class="sxs-lookup"><span data-stu-id="3228c-107">The app already shows an image and some text for each product, but the layout could be better.</span></span> <span data-ttu-id="3228c-108">Daran möchten wir jetzt arbeiten.</span><span class="sxs-lookup"><span data-stu-id="3228c-108">Let's work on that.</span></span>

1. <span data-ttu-id="3228c-109">Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **BrowseGallery1**.</span><span class="sxs-lookup"><span data-stu-id="3228c-109">In the **Screens** pane on the left, select **BrowseGallery1**.</span></span>

    <span data-ttu-id="3228c-110">Der Katalog wird daraufhin durch einen Rahmen hervorgehoben.</span><span class="sxs-lookup"><span data-stu-id="3228c-110">The selection box around the gallery confirms your choice.</span></span>

    ![Auswählen des Katalogs](../media/select-gallery.png)

1. <span data-ttu-id="3228c-112">Öffnen Sie im rechten Bereich den Bereich **Data** (Daten), indem Sie auf den Link neben **Layout** klicken.</span><span class="sxs-lookup"><span data-stu-id="3228c-112">In the right pane, open the **Data** pane by selecting the link next to **Layout**.</span></span>

    ![Anzeigen der Layoutoptionen](../media/powerapps-layout.png)

1. <span data-ttu-id="3228c-114">Wählen Sie ein anderes Layout aus, durch das z.B. das Bild, der Titel und der Untertitel werden, jedoch nicht der Text.</span><span class="sxs-lookup"><span data-stu-id="3228c-114">Select a different layout, such as the one that shows the image, the title, and the subtitle but not the body.</span></span>

    ![Ändern des Layouts](../media/change-layout.png)

1. <span data-ttu-id="3228c-116">Wählen Sie im oberen Katalogbereich die Elementkategorie aus.</span><span class="sxs-lookup"><span data-stu-id="3228c-116">Select the category of the item at the top of the gallery.</span></span>

    ![Auswählen der Kategoriebeschriftung](../media/select-category.png)

1. <span data-ttu-id="3228c-118">Ändern Sie in der Formularleiste **ThisItem.Category** in **ThisItem.Name**.</span><span class="sxs-lookup"><span data-stu-id="3228c-118">Change **ThisItem.Category** to **ThisItem.Name** in the formula bar.</span></span>

1. <span data-ttu-id="3228c-119">Wiederholen Sie die vorherigen beiden Schritte, und passen Sie dabei das andere **Beschriftungssteuerelement** so an, dass für alle Elemente Preise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="3228c-119">Repeat the previous two steps, but change the other **Label** control to show the price of each item.</span></span>

    ![Hinzufügen des Preises](../media/add-price.png)

<span data-ttu-id="3228c-121">Wie Sie sehen, können das Layout des Katalogs und die jeweiligen Datenkategorien ganz einfach angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="3228c-121">It's that easy to change the layout of a gallery and the types of data that it shows.</span></span> <span data-ttu-id="3228c-122">Vielleicht haben Sie sogar Spaß dabei.</span><span class="sxs-lookup"><span data-stu-id="3228c-122">And you might find that it's fun too!</span></span>

## <a name="details-screen"></a><span data-ttu-id="3228c-123">Detailbildschirm</span><span class="sxs-lookup"><span data-stu-id="3228c-123">Details screen</span></span>

<span data-ttu-id="3228c-124">Wir möchten die Reihenfolge der Felder auf dem Detailbildschirm ändern.</span><span class="sxs-lookup"><span data-stu-id="3228c-124">On the details screen, we want to change the order of the fields.</span></span> <span data-ttu-id="3228c-125">Die Steuerelemente auf diesem Bildschirm unterscheiden sich von den Steuerelementen auf dem Bildschirm zum Durchsuchen. Daher gibt es auch leichte Abweichungen im Änderungsprozess.</span><span class="sxs-lookup"><span data-stu-id="3228c-125">The controls on this screen differ from the controls on the browse screen, so the process for changing them is also a little different.</span></span>

1. <span data-ttu-id="3228c-126">Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **DetailScreen1** > **DetailForm1**.</span><span class="sxs-lookup"><span data-stu-id="3228c-126">On the **Screens** pane on the left, select **DetailScreen1** > **DetailForm1**.</span></span>

1. <span data-ttu-id="3228c-127">Wählen Sie im rechten Bereich den Text aus, mit dem die Anzahl der ausgewählten Felder angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3228c-127">In the right pane, select the text that shows the number of selected fields.</span></span>

    ![Auswählen des Texts, mit dem die Anzahl der ausgewählten Felder angezeigt wird](../media/powerapps-edit-fields.png)

1. <span data-ttu-id="3228c-129">Ziehen Sie das Feld **Name** in den oberen Bereich der Felderliste, und ziehen Sie das Feld **Image** (Bild) nach unten.</span><span class="sxs-lookup"><span data-stu-id="3228c-129">Drag the **Name** field to the top of the list of fields, and drag the **Image** field to the bottom.</span></span>

    ![Bewegen von Feldern auf dem Detailbildschirm](../media/powerapps-move-fields.png)

## <a name="editcreate-screen"></a><span data-ttu-id="3228c-131">Bildschirm zum Bearbeiten/Erstellen</span><span class="sxs-lookup"><span data-stu-id="3228c-131">Edit/create screen</span></span>

<span data-ttu-id="3228c-132">Abschließend soll nun auf dem Bildschirm, auf dem Benutzer Einträge erstellen und bearbeiten, die Eingabe von Informationen im Textfeld erleichtert werden.</span><span class="sxs-lookup"><span data-stu-id="3228c-132">Finally, on the screen where your user edits and creates entries, we want to make it easier to enter information in a text box.</span></span>

1. <span data-ttu-id="3228c-133">Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **EditScreen1** > **EditForm1**.</span><span class="sxs-lookup"><span data-stu-id="3228c-133">On the **Screens** pane on the left, select **EditScreen1** > **EditForm1**.</span></span>

1. <span data-ttu-id="3228c-134">Wählen Sie im rechten Bereich den Text aus, mit dem die Anzahl der ausgewählten Felder angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3228c-134">In the right pane, select the text that shows the number of selected fields.</span></span>

1. <span data-ttu-id="3228c-135">Klicken Sie zuerst auf den Dropdownpfeil der Liste **Overview** (Übersicht) und anschließend auf **Mehrzeiligen Text bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="3228c-135">Select the drop-down arrow for the **Overview** list, and then select **Edit multi-line text**.</span></span>

    <span data-ttu-id="3228c-136">Mit dem Bearbeitungssteuerelement für mehrzeiligen Text wird die Eingabe längerer Texte vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="3228c-136">A multi-line edit control will make it easier to add more than a few words in this field.</span></span>

    ![Ändern von Feldern für den Bildschirm zum Erstellen/Bearbeiten](../media/powerapps-change-editscreen.png)

<span data-ttu-id="3228c-138">Nun wissen Sie, wie die Darstellung und Benutzerfreundlichkeit einer erstellten App mit einigen grundlegenden Schritten erheblich verbessert werden kann.</span><span class="sxs-lookup"><span data-stu-id="3228c-138">You've seen how a few basic steps can do a lot to improve the appearance and experience of using an app.</span></span> <span data-ttu-id="3228c-139">In dieser Einheit haben Sie sich auf die Anwendung PowerApps Studio konzentriert, die viele Optionen zum Anpassen von Apps bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="3228c-139">In this unit, we focused on PowerApps Studio, which provides lots of options for customizing apps.</span></span> <span data-ttu-id="3228c-140">In der nächsten Einheit werden die Steuerelemente der App ausführlicher dargestellt.</span><span class="sxs-lookup"><span data-stu-id="3228c-140">In the next unit, we'll explore the controls in the app in greater detail.</span></span>