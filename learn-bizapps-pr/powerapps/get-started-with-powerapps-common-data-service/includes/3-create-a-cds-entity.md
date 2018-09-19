<span data-ttu-id="58c61-101">In dieser Lektion erstellen Sie eine Entität und passen anschließend wichtige Komponenten wie Felder, Beziehungen, Ansichten und Formulare an.</span><span class="sxs-lookup"><span data-stu-id="58c61-101">In this unit, you'll create an entity and then customize key components, like fields, relationships, views, and forms.</span></span> <span data-ttu-id="58c61-102">Sie lernen Folgendes:</span><span class="sxs-lookup"><span data-stu-id="58c61-102">You'll learn how to:</span></span>

- <span data-ttu-id="58c61-103">Erstellen einer benutzerdefinierten Entität</span><span class="sxs-lookup"><span data-stu-id="58c61-103">Create a custom entity.</span></span>
- <span data-ttu-id="58c61-104">Hinzufügen benutzerdefinierter Felder zur Entität</span><span class="sxs-lookup"><span data-stu-id="58c61-104">Add custom fields to your entity.</span></span>
- <span data-ttu-id="58c61-105">Hinzufügen einer Entitätsbeziehung</span><span class="sxs-lookup"><span data-stu-id="58c61-105">Add an entity relationship.</span></span>
- <span data-ttu-id="58c61-106">Anpassen einer Ansicht</span><span class="sxs-lookup"><span data-stu-id="58c61-106">Customize a view.</span></span>
- <span data-ttu-id="58c61-107">Anpassen eines Formulars</span><span class="sxs-lookup"><span data-stu-id="58c61-107">Customize a form.</span></span>

<span data-ttu-id="58c61-108">Dieses Tutorial orientiert sich am Unternehmen Contoso, das einen Haustierpflegedienst für Hunde und Katzen betreibt.</span><span class="sxs-lookup"><span data-stu-id="58c61-108">The tutorial follows the Contoso company, which is a pet grooming business that grooms dogs and cats.</span></span> <span data-ttu-id="58c61-109">Contoso benötigt eine App zum Nachverfolgen von Kunden und Haustieren, die von den Mitarbeitern auf einer Vielzahl von Geräten genutzt werden kann.</span><span class="sxs-lookup"><span data-stu-id="58c61-109">Contoso needs an app for client and pet tracking that can be used by employees on a variety of devices.</span></span>

## <a name="create-a-custom-entity"></a><span data-ttu-id="58c61-110">Erstellen einer benutzerdefinierten Entität</span><span class="sxs-lookup"><span data-stu-id="58c61-110">Create a custom entity</span></span>

1. <span data-ttu-id="58c61-111">Erweitern Sie im linken Navigationsbereich **Daten**. Wählen Sie **Entitäten** und dann **Neue Entität** erstellen aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-111">In the left navigation pane, expand **Data**, select **Entities**, and then select **New entity**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-112">![Neue Entität](../media/create-new-entity.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-112">![New entity](../media/create-new-entity.png)</span></span>

2. <span data-ttu-id="58c61-113">Geben Sie die folgenden Werte ein:</span><span class="sxs-lookup"><span data-stu-id="58c61-113">Enter the following values:</span></span>

    - <span data-ttu-id="58c61-114">**Anzeigename**: *Haustier*</span><span class="sxs-lookup"><span data-stu-id="58c61-114">**Display name**: *Pet*</span></span>
    - <span data-ttu-id="58c61-115">**Beschreibung**: *Benutzerdefinierte Entität zum Nachverfolgen von Dienstleistungen für Haustiere*</span><span class="sxs-lookup"><span data-stu-id="58c61-115">**Description**: *Custom entity to track pet services*</span></span>

3. <span data-ttu-id="58c61-116">Klicken Sie auf **Weiter**, und wählen Sie dann, nachdem die Standardfelder eingeblendet wurden, **Entität speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-116">Select **Next**, and then, after the default fields are shown, select **Save Entity**.</span></span>

## <a name="add-and-customize-fields"></a><span data-ttu-id="58c61-117">Hinzufügen und Anpassen von Feldern</span><span class="sxs-lookup"><span data-stu-id="58c61-117">Add and customize fields</span></span>

1. <span data-ttu-id="58c61-118">Wählen Sie in der Liste der Entitäten die Entität **Haustier** aus, die Sie im vorherigen Abschnitt erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="58c61-118">In the list of entities, select the **Pet** entity that you created in the previous section.</span></span>
2. <span data-ttu-id="58c61-119">Wählen Sie auf der Registerkarte **Felder** das Feld **Haustier** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-119">On the **Fields** tab, select the **Pet** field.</span></span>
3. <span data-ttu-id="58c61-120">Nehmen Sie im rechten Bereich folgende Änderungen am Feld **Anzeigename** vor:</span><span class="sxs-lookup"><span data-stu-id="58c61-120">In the right pane, make the following changes to the **Display name** field:</span></span>

    - <span data-ttu-id="58c61-121">Ändern Sie den Wert **Anzeigename** von *Haustier* in *Name des Haustiers*.</span><span class="sxs-lookup"><span data-stu-id="58c61-121">Change the **Display name** value from *Pet* to *Pet Name*.</span></span>
    - <span data-ttu-id="58c61-122">Aktivieren Sie das Kontrollkästchen **Durchsuchbar**.</span><span class="sxs-lookup"><span data-stu-id="58c61-122">Select **Searchable**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-123">![Primäres Feld ändern](../media/primary-field.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-123">![Change primary field](../media/primary-field.png)</span></span>

3. <span data-ttu-id="58c61-124">Klicken Sie auf **Fertig**.</span><span class="sxs-lookup"><span data-stu-id="58c61-124">Select **Done**.</span></span>
4. <span data-ttu-id="58c61-125">Klicken Sie auf der Registerkarte **Felder** auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-125">On the **Fields** tab, on the entity designer toolbar, select **Add field**.</span></span>
5. <span data-ttu-id="58c61-126">Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein:</span><span class="sxs-lookup"><span data-stu-id="58c61-126">In the **Field properties** pane, enter the following values:</span></span>

    - <span data-ttu-id="58c61-127">**Anzeigename**: *Art*</span><span class="sxs-lookup"><span data-stu-id="58c61-127">**Display name**: *Species*</span></span>
    - <span data-ttu-id="58c61-128">**Datentyp**: *Optionssatz*</span><span class="sxs-lookup"><span data-stu-id="58c61-128">**Data type**: *Option Set*</span></span>
    - <span data-ttu-id="58c61-129">**Optionssatz**: *Neuer Optionssatz*</span><span class="sxs-lookup"><span data-stu-id="58c61-129">**Option set**: *New option set*</span></span>

6. <span data-ttu-id="58c61-130">Erstellen Sie den Optionssatz:</span><span class="sxs-lookup"><span data-stu-id="58c61-130">Create the option set:</span></span>

    1. <span data-ttu-id="58c61-131">Klicken Sie auf **Neues Element hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-131">Select **Add new item**.</span></span>
    2. <span data-ttu-id="58c61-132">Ersetzen Sie *Neue Option* durch *Hund*.</span><span class="sxs-lookup"><span data-stu-id="58c61-132">Replace *New option* with *Dog*.</span></span>
    3. <span data-ttu-id="58c61-133">Klicken Sie auf **Neues Element hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-133">Select **Add new item**.</span></span>
    4. <span data-ttu-id="58c61-134">Ersetzen Sie *Neue Option* durch *Katze*.</span><span class="sxs-lookup"><span data-stu-id="58c61-134">Replace *New option* with *Cat*.</span></span>
    5. <span data-ttu-id="58c61-135">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="58c61-135">Select **Save**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-136">![Neuer Optionssatz](../media/optionset-add-items.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-136">![New option set](../media/optionset-add-items.png)</span></span>

7. <span data-ttu-id="58c61-137">Aktivieren Sie **Durchsuchbar**, und klicken Sie dann auf **Fertig**.</span><span class="sxs-lookup"><span data-stu-id="58c61-137">Select **Searchable**, and then select **Done**.</span></span>
8. <span data-ttu-id="58c61-138">Klicken auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-138">On the entity designer toolbar, select **Add field**.</span></span>
9. <span data-ttu-id="58c61-139">Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein, und klicken Sie dann auf **Fertig**:</span><span class="sxs-lookup"><span data-stu-id="58c61-139">In the **Field properties** pane, enter the following values, and then select **Done**:</span></span>

    - <span data-ttu-id="58c61-140">**Anzeigename**: *Rasse*</span><span class="sxs-lookup"><span data-stu-id="58c61-140">**Display name**: *Breed*</span></span>
    - <span data-ttu-id="58c61-141">**Datentyp**: *Text*</span><span class="sxs-lookup"><span data-stu-id="58c61-141">**Data type**: *Text*</span></span>
    - <span data-ttu-id="58c61-142">**Durchsuchbar**: *Ja*</span><span class="sxs-lookup"><span data-stu-id="58c61-142">**Searchable**: *Yes*</span></span>

10. <span data-ttu-id="58c61-143">Klicken auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-143">On the entity designer toolbar, select **Add field**.</span></span>
11. <span data-ttu-id="58c61-144">Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein, und klicken Sie dann auf **Fertig**:</span><span class="sxs-lookup"><span data-stu-id="58c61-144">In the **Field properties** pane, enter the following values, and then select **Done**:</span></span>

    - <span data-ttu-id="58c61-145">**Anzeigename**: *Datum des Termins*</span><span class="sxs-lookup"><span data-stu-id="58c61-145">**Display name**: *Appointment date*</span></span>
    - <span data-ttu-id="58c61-146">**Datentyp**: *Datum und Uhrzeit*</span><span class="sxs-lookup"><span data-stu-id="58c61-146">**Data type**: *Date and time*</span></span>

12. <span data-ttu-id="58c61-147">Klicken Sie auf **Entität speichern**.</span><span class="sxs-lookup"><span data-stu-id="58c61-147">Select **Save Entity**.</span></span>

## <a name="add-a-relationship"></a><span data-ttu-id="58c61-148">Hinzufügen einer Beziehung</span><span class="sxs-lookup"><span data-stu-id="58c61-148">Add a relationship</span></span>

1. <span data-ttu-id="58c61-149">Klicken Sie auf der Registerkarte **Beziehungen** auf der Entity Designer-Symbolleiste auf **Beziehung hinzufügen**, und wählen Sie dann **n:1** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-149">On the **Relationships** tab, on the entity designer toolbar, select **Add relationship**, and then select **Many-to-one**.</span></span>
2. <span data-ttu-id="58c61-150">Wählen Sie im rechten Bereich in der Liste **Verknüpft** den Eintrag **Konto** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-150">In the right pane, in the **Related** list, select **Account**.</span></span>
3. <span data-ttu-id="58c61-151">Klicken Sie auf **Fertig**.</span><span class="sxs-lookup"><span data-stu-id="58c61-151">Select **Done**.</span></span>
4. <span data-ttu-id="58c61-152">Klicken Sie auf **Entität speichern**.</span><span class="sxs-lookup"><span data-stu-id="58c61-152">Select **Save Entity**.</span></span>

    <span data-ttu-id="58c61-153">Beachten Sie, dass beim Hinzufügen einer n-:1-Beziehung ein Feld des Typs **Konto** mit dem Datentyp **Suche** automatisch zu Ihrer Liste der Felder auf der Registerkarte **Felder** hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="58c61-153">Notice that when you add a many-to-one relationship, an **Account** field of the **Lookup** data type is automatically added to your list of fields on the **Fields** tab.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-154">![Feld zum Suchen eines Kontos](../media/account-lookup-field.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-154">![Account lookup field](../media/account-lookup-field.png)</span></span>

## <a name="customize-a-view"></a><span data-ttu-id="58c61-155">Anpassen einer Ansicht</span><span class="sxs-lookup"><span data-stu-id="58c61-155">Customize a view</span></span>

1. <span data-ttu-id="58c61-156">Wählen Sie auf der Registerkarte **Ansichten** die Ansicht **Aktive Haustiere** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-156">On the **Views** tab, select the **Active Pets** view.</span></span> <span data-ttu-id="58c61-157">Wenn die Ansicht **Aktive Haustiere** nicht angezeigt wird, wählen **Filter entfernen** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-157">If you don't see the **Active Pets** view, select **Remove filter**.</span></span>
2. <span data-ttu-id="58c61-158">Wählen Sie im Ansicht-Designer **Spalten hinzufügen** und dann die folgenden Spalten aus. Klicken Sie anschließend auf **OK**:</span><span class="sxs-lookup"><span data-stu-id="58c61-158">In the view designer, select **Add Columns**, select the following columns, and then select **OK**:</span></span>

    - <span data-ttu-id="58c61-159">Konto</span><span class="sxs-lookup"><span data-stu-id="58c61-159">Account</span></span>
    - <span data-ttu-id="58c61-160">Datum des Termins</span><span class="sxs-lookup"><span data-stu-id="58c61-160">Appointment date</span></span>
    - <span data-ttu-id="58c61-161">Rasse</span><span class="sxs-lookup"><span data-stu-id="58c61-161">Breed</span></span>
    - <span data-ttu-id="58c61-162">Art</span><span class="sxs-lookup"><span data-stu-id="58c61-162">Species</span></span>

3. <span data-ttu-id="58c61-163">Klicken Sie auf die Spalte **Erstellt am**, dann auf **Entfernen** und anschließend auf **OK**, um das Entfernen der Spalte zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="58c61-163">Select the **Created On** column, select **Remove**, and then select **OK** to confirm the column removal.</span></span>
4. <span data-ttu-id="58c61-164">Um die Spalten anzuordnen, wählen Sie die zu verschiebende Spalte aus, und klicken Sie dann auf die Pfeiltasten (**\<-** und **-\>**), bis Ihre Ansicht so aussieht.</span><span class="sxs-lookup"><span data-stu-id="58c61-164">To arrange the columns, select the column to move, and then use the arrow buttons (**\<-** and **-\>**) until your view looks like this.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-165">![Ansicht „Aktive Haustiere“](../media/active-pets-view.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-165">![Active pets view](../media/active-pets-view.png)</span></span>

5. <span data-ttu-id="58c61-166">Klicken Sie auf der Symbolleiste des Ansicht-Designers auf **Speichern und schließen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-166">On the view designer toolbar, select **Save and Close**.</span></span>

## <a name="customize-the-main-form"></a><span data-ttu-id="58c61-167">Anpassen des Hauptformulars</span><span class="sxs-lookup"><span data-stu-id="58c61-167">Customize the main form</span></span>

1. <span data-ttu-id="58c61-168">Wählen Sie in PowerApps im linken Navigationsbereich **Modellgesteuert** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-168">In PowerApps, in the left navigation pane, select **Model-driven**.</span></span>
2. <span data-ttu-id="58c61-169">Erweitern Sie im linken Navigationsbereich **Daten**. Wählen Sie **Entitäten** und dann **Haustier** aus.</span><span class="sxs-lookup"><span data-stu-id="58c61-169">In the left navigation pane, expand **Data**, select **Entities**, and then select **Pet**.</span></span>
3. <span data-ttu-id="58c61-170">Wählen Sie auf der Registerkarte **Formulare** den Eintrag **Informationen** neben dem Typ **Hauptformular** aus, um den Formular-Editor zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="58c61-170">On the **Forms** tab, select **Information** next to the **Main** form type to open the form editor.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-171">![Bearbeiten des Hauptformulars](../media/main-form-edit.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-171">![Edit main form](../media/main-form-edit.png)</span></span>

4. <span data-ttu-id="58c61-172">Ziehen Sie im Formular-Editor die Felder **Art**, **Rasse**, **Datum des Termins** und **Konto** aus dem Bereich **Feld-Explorer** in den Abschnitt **Allgemein** des Formularzeichenbereichs, bis das Formular so aussieht.</span><span class="sxs-lookup"><span data-stu-id="58c61-172">In the form editor, drag the **Species**, **Breed**, **Appointment date**, and **Account** fields from the **Field Explorer** pane to the **General** section of the form canvas, so that the form looks like this.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="58c61-173">![Auswählen von Feldern für das Hauptformular](../media/main-form-edit2.png)</span><span class="sxs-lookup"><span data-stu-id="58c61-173">![Select fields for main form](../media/main-form-edit2.png)</span></span>

5. <span data-ttu-id="58c61-174">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="58c61-174">Select **Save**.</span></span>
6. <span data-ttu-id="58c61-175">Klicken Sie auf **Veröffentlichen**.</span><span class="sxs-lookup"><span data-stu-id="58c61-175">Select **Publish**.</span></span>
7. <span data-ttu-id="58c61-176">Klicken Sie auf **Speichern und schließen**, um den Formulardesigner zu schließen.</span><span class="sxs-lookup"><span data-stu-id="58c61-176">Select **Save and close** to close the form designer.</span></span>
