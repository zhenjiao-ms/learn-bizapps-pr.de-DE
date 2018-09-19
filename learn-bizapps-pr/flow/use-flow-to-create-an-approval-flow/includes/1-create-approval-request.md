<span data-ttu-id="5269c-101">In dieser Einheit erfahren Sie, wie Sie ein für Unternehmen geeignetes Szenario erstellen, in dem Genehmigungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5269c-101">In this unit, you'll learn how to build a business-friendly scenario that uses approvals.</span></span>

<span data-ttu-id="5269c-102">In diesem Szenario kann jede Person mit Zugriff auf die Microsoft SharePoint-Liste Tweets verfassen, ohne mit Twitter vertraut zu sein.</span><span class="sxs-lookup"><span data-stu-id="5269c-102">In this scenario, anyone who has access to the Microsoft SharePoint list can contribute tweets without knowing anything about Twitter.</span></span> <span data-ttu-id="5269c-103">Das Social-Media-Team kann die Tweets anschließend genehmigen oder ablehnen.</span><span class="sxs-lookup"><span data-stu-id="5269c-103">The social media team can then approve or reject those tweets.</span></span> <span data-ttu-id="5269c-104">Dadurch wird die Kontrolle über das Konto und alle Inhalte sichergestellt, die für Kunden freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5269c-104">That team maintains control of the account and the content that goes out to customers.</span></span> 

## <a name="step-one-create-a-sharepoint-list-for-tweets"></a><span data-ttu-id="5269c-105">Schritt 1: Erstellen einer SharePoint-Liste für Tweets</span><span class="sxs-lookup"><span data-stu-id="5269c-105">Step one: Create a SharePoint list for tweets</span></span>

<span data-ttu-id="5269c-106">Sie verwenden im Folgenden eine Vorlage, durch die ein Genehmigungsprozess gestartet wird, wenn ein neues Element in einer Liste erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="5269c-106">You'll use a template that starts an approval process whenever a new item is created in a specific list.</span></span> <span data-ttu-id="5269c-107">Wird das Element genehmigt, wird ein Tweet auf Twitter gepostet.</span><span class="sxs-lookup"><span data-stu-id="5269c-107">If the item is approved, a tweet is then posted to Twitter.</span></span> <span data-ttu-id="5269c-108">In dieser Einheit ändern Sie den Vorgang, indem Sie Schritte hinzufügen, die die SharePoint-Liste mit der Genehmigungsantwort aktualisieren. Zusätzlich zeigen diese Schritte an, ob ein Element genehmigt wurde, und fügen Kommentare ein, die dem vorgeschlagenen Tweet von der genehmigenden Person hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="5269c-108">For this unit, you'll change the process by adding steps that update a SharePoint list with the approval response, indicate whether the item was approved, and add any comments that the approver added to the proposed tweet.</span></span> 

<span data-ttu-id="5269c-109">Im Folgenden erstellen Sie zunächst die SharePoint-Liste.</span><span class="sxs-lookup"><span data-stu-id="5269c-109">First, let's create the SharePoint list.</span></span>

1. <span data-ttu-id="5269c-110">Erstellen Sie auf Ihrer SharePoint-Website eine SharePoint-Liste mit dem Namen **Contoso-Tweets**.</span><span class="sxs-lookup"><span data-stu-id="5269c-110">On your SharePoint site, create a SharePoint list named **ContosoTweets**.</span></span>
1. <span data-ttu-id="5269c-111">Öffnen Sie die Liste, und klicken Sie auf **Spalte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="5269c-111">Open the list, and select **Add column**.</span></span>
1. <span data-ttu-id="5269c-112">Klicken Sie auf **+ Spalte hinzufügen**, um die folgenden Spalten hinzuzufügen:</span><span class="sxs-lookup"><span data-stu-id="5269c-112">Select **+ Add column** to add the following columns:</span></span>

    - <span data-ttu-id="5269c-113">Fügen Sie eine **Tweetinhalt**-Spalte hinzu, und legen Sie als Spaltentyp **Multiple lines of text** (Mehrere Textzeilen) fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-113">Add a **TweetContent** column, and set the column type to **Multiple lines of text**.</span></span> <span data-ttu-id="5269c-114">Diese Spalte enthält den Inhalt der Tweets, die später genehmigt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="5269c-114">This will contain the content of the tweets for later approval.</span></span> <span data-ttu-id="5269c-115">Klicken Sie nach dem Erstellen einer Spalte immer auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="5269c-115">Select **Save** after each column you create.</span></span>
    - <span data-ttu-id="5269c-116">Fügen Sie eine **Tweetdatum**-Spalte hinzu, und legen Sie als Spaltentyp **Datum und Uhrzeit** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-116">Add a **TweetDate** column, and set the column type to **Date and Time**.</span></span> <span data-ttu-id="5269c-117">Klicken Sie auf **More** (Weitere), damit der Typ **Datum und Uhrzeit** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5269c-117">Select **More** to find the **Date and Time** type.</span></span>
    - <span data-ttu-id="5269c-118">Fügen Sie die Spalte **Genehmigungsstatus** hinzu, und legen Sie als Spaltentyp **Ja/Nein** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-118">Add an **ApprovalStatus** column, and set the column type to **Yes/No**.</span></span> <span data-ttu-id="5269c-119">Die genehmigende Person kann dann **Ja** oder **Nein** auswählen, um den Tweet zu genehmigen oder abzulehnen.</span><span class="sxs-lookup"><span data-stu-id="5269c-119">The approver can then select **Yes** or **No** to approve or reject the tweet.</span></span>
    - <span data-ttu-id="5269c-120">Fügen Sie die Spalte **Kommentare der genehmigenden Person** hinzu, und legen Sie als Spaltentyp **Einzelne Textzeile** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-120">Add an **ApproverComments** column, and set the column type to **Single line of text**.</span></span> <span data-ttu-id="5269c-121">Die genehmigende Person kann dadurch einen Kommentar zum Genehmigungsstatus hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="5269c-121">The approver can then add a comment about the approval status.</span></span>

    ![Hinzufügen von Spalten](../media/new-columns.png)

1. <span data-ttu-id="5269c-123">Kopieren Sie die URL der SharePoint-Liste.</span><span class="sxs-lookup"><span data-stu-id="5269c-123">Copy the URL of the SharePoint list.</span></span> <span data-ttu-id="5269c-124">Die URL verwenden Sie bei der Erstellung des Flows.</span><span class="sxs-lookup"><span data-stu-id="5269c-124">You'll use it when you create the flow.</span></span>

## <a name="step-two-create-an-approval-request-flow"></a><span data-ttu-id="5269c-125">Schritt 2: Erstellen eines Flows für die Genehmigungsanforderung</span><span class="sxs-lookup"><span data-stu-id="5269c-125">Step two: Create an approval request flow</span></span>
1. <span data-ttu-id="5269c-126">Melden Sie sich bei [Microsoft Flow](https://ms.flow.microsoft.com) an, und wählen Sie **Genehmigungen** aus.</span><span class="sxs-lookup"><span data-stu-id="5269c-126">Sign in to [Microsoft Flow](https://ms.flow.microsoft.com), and then select **Approvals**.</span></span>

1. <span data-ttu-id="5269c-127">Klicken Sie auf **Genehmigungsflow erstellen**, scrollen Sie nach unten, und wählen Sie die Vorlage **Listenelemente nach Genehmigung in Twitter posten** aus.</span><span class="sxs-lookup"><span data-stu-id="5269c-127">Select **Create approval flow**, and then scroll down and select the **Post list items to Twitter after approval** template.</span></span> 

    ![Auswählen der Vorlage](../media/create-approval.png)

1. <span data-ttu-id="5269c-129">Stellen Sie sicher, dass Ihre Kontoanmeldeinformationen für **SharePoint**, **Genehmigungen** und **Twitter** richtig sind, und klicken Sie dann auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="5269c-129">Make sure your account credentials for **SharePoint**, **Approvals**, and **Twitter** are correct, and then select **Continue**.</span></span> 

    ![Überprüfen von Anmeldeinformationen](../media/verify-credentials.png)

1. <span data-ttu-id="5269c-131">Geben Sie in Microsoft Flow in der Aktion **Wenn ein neues Element erstellt wird** die folgenden Werte ein:</span><span class="sxs-lookup"><span data-stu-id="5269c-131">Back in Microsoft Flow, in the **When a new item is created** action, enter the following values:</span></span>

    * <span data-ttu-id="5269c-132">**Websiteadresse:** Geben Sie die URL der SharePoint-Website Ihres Teams ein.</span><span class="sxs-lookup"><span data-stu-id="5269c-132">**Site Address**: Enter the URL of your team's SharePoint site.</span></span>
    * <span data-ttu-id="5269c-133">**Listenname:** Wählen Sie *ContosoTweets* aus.</span><span class="sxs-lookup"><span data-stu-id="5269c-133">**List Name**: Select *ContosoTweets*.</span></span>

    ![Websiteadresse und Listenname](../media/site-address.png)

1. <span data-ttu-id="5269c-135">Klicken Sie in der Aktion **Start an approval** (Genehmigungsflow starten) auf **Bearbeiten**, damit alle Felder angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5269c-135">In the **Start an approval** action, select **Edit** to show all the fields.</span></span> 

    ![Bearbeiten von Feldern](../media/edit-all-fields.png)

1. <span data-ttu-id="5269c-137">Geben Sie *Neuer Tweet für* als **Titel** ein, und wählen Sie dann **Titel** in der Liste für dynamische Inhalte aus.</span><span class="sxs-lookup"><span data-stu-id="5269c-137">For **Title**, enter *New tweet for*, and then select **Title** in the dynamic content list.</span></span> 

    ![Titel](../media/tweet-title.png)

1. <span data-ttu-id="5269c-139">Geben Sie bei **Zugewiesen an** entweder Ihren Namen oder den eines Testbenutzers ein, und wählen Sie diesen Namen aus.</span><span class="sxs-lookup"><span data-stu-id="5269c-139">For **Assigned to**, enter and select either your name or a test user name.</span></span> 

    ![Zugewiesen an](../media/tweet-assigned-to.png)

1. <span data-ttu-id="5269c-141">Entfernen Sie bei **Details** die Standardelemente, und fügen Sie **Tweetinhalt**, **Tweetdatum** und **Erstellt von Anzeigename** aus der Liste für dynamische Inhalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="5269c-141">For **Details**, remove the default items, and add **TweetContent**, **TweetDate**, and **Created by DisplayName** from the dynamic content list.</span></span> <span data-ttu-id="5269c-142">Achten Sie bei der Eingabe darauf, Bezüge durch Wörter wie *von* deutlich zu machen, damit der Inhalt leichter verständlich ist.</span><span class="sxs-lookup"><span data-stu-id="5269c-142">Be sure to add the words *on* and *by* to make the content more readable.</span></span> 

    ![Details](../media/tweet-details.png)

1. <span data-ttu-id="5269c-144">Fügen Sie bei **Elementlink** die URL der SharePoint-Liste ein, die Sie in **Schritt 1** kopiert haben.</span><span class="sxs-lookup"><span data-stu-id="5269c-144">For **Item Link**, paste the URL of your SharePoint list, which you copied in the procedure in **Step one**.</span></span> <span data-ttu-id="5269c-145">Geben Sie *Contoso-Tweetliste* als **Beschreibung des Elementlinks** ein.</span><span class="sxs-lookup"><span data-stu-id="5269c-145">For **Item Link Description**, enter *Contoso Tweet List*.</span></span> 

    ![Elementlink](../media/tweet-item-link.png)

1. <span data-ttu-id="5269c-147">Zeigen Sie in der Aktion **Bedingung** auf das Feld **WENN JA**, und klicken Sie anschließend zuerst auf das Pluszeichen (**+**) und dann auf **Aktion hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="5269c-147">In the **Condition** action, hover over the **IF YES** box, select the plus sign (**+**), and then select **Add an action**.</span></span> 

    ![Hinzufügen einer Aktion](../media/add-an-action.png)

1. <span data-ttu-id="5269c-149">Suchen Sie nach *Element aktualisieren*, und klicken Sie anschließend zuerst auf den **SharePoint-Connector** und dann auf die Aktion **SharePoint – Element aktualisieren**.</span><span class="sxs-lookup"><span data-stu-id="5269c-149">Search for *update item*, select the **SharePoint** connector, and then select the **SharePoint – Update item** action.</span></span>

    ![SharePoint – Element aktualisieren](../media/update-item.png)

1. <span data-ttu-id="5269c-151">Geben Sie bei **Websiteadresse** und **Listenname** erneut die SharePoint-Website-URL des Teams und *Contoso-Tweets* ein.</span><span class="sxs-lookup"><span data-stu-id="5269c-151">For **Site Address** and **List Name**, enter the URL of the team's SharePoint site and *ContosoTweets* again.</span></span> <span data-ttu-id="5269c-152">Fügen Sie bei **ID** die **ID** aus der Liste für dynamische Inhalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="5269c-152">For **ID**, add **ID** from the dynamic content list.</span></span> <span data-ttu-id="5269c-153">Mit dem **ID**-Feld wird versucht, für die Anforderung für den eigentlichen Tweet in der SharePoint-Liste eine Übereinstimmung zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="5269c-153">The **ID** field is used to match the actual tweet request in the SharePoint list.</span></span>

    ![Website, Liste und ID](../media/address-list-id.png)

1. <span data-ttu-id="5269c-155">Klicken Sie auf das Feld **Titel**, und suchen Sie in der Liste für dynamische Inhalte nach *Titel*.</span><span class="sxs-lookup"><span data-stu-id="5269c-155">Select the **Title** field, and then, in the dynamic content list, search for *title*.</span></span> <span data-ttu-id="5269c-156">Fügen Sie das **Titel**-Element über die Aktion **Wenn ein neues Element erstellt wird** hinzu.</span><span class="sxs-lookup"><span data-stu-id="5269c-156">Add the **Title** item from the **When a new item is created** action.</span></span> 

    ![Neuer Titel](../media/add-title.png)

1. <span data-ttu-id="5269c-158">Wählen Sie **Genehmigungsstatus** aus, und legen Sie als Wert **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-158">Select **ApprovalStatus**, and set the value to **Yes**.</span></span> <span data-ttu-id="5269c-159">Wählen Sie anschließend **Kommentare der genehmigenden Person** aus, und legen Sie den Wert über die Liste für dynamische Inhalte auf **Kommentare** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-159">Then select **ApproverComments**, and set the value to **Comments** from the dynamic content list.</span></span> 

    ![Status und Kommentare](../media/approver-status.png)

1. <span data-ttu-id="5269c-161">Klicken Sie im unteren Bereich des Felds **IF NO, DO NOTHING** (WENN NEIN, KEINE AKTION AUSFÜHREN) auf **Aktion hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="5269c-161">Near the bottom of the **IF NO, DO NOTHING** box, select **Add an action**.</span></span>

    ![Hinzufügen einer Aktion mit Genehmigungsstatus „Nein“](../media/add-a-no-action.png)

1. <span data-ttu-id="5269c-163">Wiederholen Sie die Schritte 11 bis 14, um eine Aktion des Typs **SharePoint – Element aktualisieren** zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="5269c-163">Repeat steps 11 through 14 to create a **SharePoint – Update item** action.</span></span> <span data-ttu-id="5269c-164">Legen Sie die gleichen Werte wie für die **WENN JA**-Bedingung fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-164">Set the same values you set for the **IF YES** condition.</span></span> <span data-ttu-id="5269c-165">Die einzige Ausnahme ist **Genehmigungsstatus**, da Sie für diesen **Nein** festlegen.</span><span class="sxs-lookup"><span data-stu-id="5269c-165">The only difference is that you should set **ApprovalStatus** to **No**.</span></span> 

    ![Genehmigungsstatus = Nein](../media/status-no.png)

1. <span data-ttu-id="5269c-167">Wählen Sie die Aktion **Tweet posten** aus, klicken Sie auf **Bearbeiten**, und legen Sie mithilfe der Liste für dynamische Inhalte für **Tweettext** den Wert **Tweetinhalt** fest.</span><span class="sxs-lookup"><span data-stu-id="5269c-167">Select the **Post a tweet** action, select **Edit**, and set **Tweet text** to **TweetContent** from the dynamic content list.</span></span> <span data-ttu-id="5269c-168">Dadurch wird der eigentliche Tweet erstellt und nach dessen Genehmigung auf Twitter gepostet.</span><span class="sxs-lookup"><span data-stu-id="5269c-168">This will create the actual tweet and then post it to Twitter when it's approved.</span></span> 

    ![Posten und Speichern](../media/post-tweet.png)

1. <span data-ttu-id="5269c-170">Klicken Sie auf **Flow erstellen**.</span><span class="sxs-lookup"><span data-stu-id="5269c-170">Select **Create flow**.</span></span>

<span data-ttu-id="5269c-171">Herzlichen Glückwunsch!</span><span class="sxs-lookup"><span data-stu-id="5269c-171">Congratulations!</span></span> <span data-ttu-id="5269c-172">Sie haben Ihren ersten Flow erstellt.</span><span class="sxs-lookup"><span data-stu-id="5269c-172">You just created your first flow.</span></span> 

<span data-ttu-id="5269c-173">Microsoft Flow bietet Ihnen noch mehr Möglichkeiten, die Produktivität Ihres Teams zu steigern.</span><span class="sxs-lookup"><span data-stu-id="5269c-173">This is just one way that Microsoft Flow can empower your team to be more productive.</span></span> <span data-ttu-id="5269c-174">Ihr Team kann Vorschläge, wichtige Neuigkeiten oder Produktanleitungen bereitstellen. Dabei können Sie allerdings immer festlegen, welche Tweets für Kunden freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5269c-174">Your team can contribute ideas, relevant news, or product guidance, but you still maintain control over what's tweeted out to customers.</span></span>

<span data-ttu-id="5269c-175">In der nächsten Einheit wird beschrieben, was geschieht, wenn die genehmigende Person eine neue Anforderung für einen vorgeschlagenen Tweet empfängt.</span><span class="sxs-lookup"><span data-stu-id="5269c-175">In the next unit, you'll see what it looks like when an approver receives a new request for a proposed tweet.</span></span>