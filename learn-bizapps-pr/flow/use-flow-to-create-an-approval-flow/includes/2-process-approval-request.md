<span data-ttu-id="36d92-101">In der vorherigen Einheit haben Sie erfahren, wie Sie einen Genehmigungsprozess für Tweets erstellen, die in einer Microsoft SharePoint-Liste gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="36d92-101">In the previous unit, you learned how to build an approval process for tweets that are stored in a Microsoft SharePoint list.</span></span> <span data-ttu-id="36d92-102">In dieser Einheit wird beschrieben, was geschieht, wenn eine genehmigende Person eine neue Genehmigungsanforderung empfängt.</span><span class="sxs-lookup"><span data-stu-id="36d92-102">In this unit, you'll see what the experience looks like when an approver receives a new approval request.</span></span> 

## <a name="step-one-change-the-sharepoint-list"></a><span data-ttu-id="36d92-103">Schritt 1: Anpassen der SharePoint-Liste</span><span class="sxs-lookup"><span data-stu-id="36d92-103">Step one: Change the SharePoint list</span></span>
<span data-ttu-id="36d92-104">Zunächst fügen Sie Ihrer SharePoint-Liste ein Element hinzu.</span><span class="sxs-lookup"><span data-stu-id="36d92-104">First, we need to add an item to our SharePoint list.</span></span> <span data-ttu-id="36d92-105">Anschließend kann eine Genehmigungsanforderung für dieses Element verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="36d92-105">We can then process an approval request for that item.</span></span>

1. <span data-ttu-id="36d92-106">Öffnen Sie in SharePoint die **Contoso-Tweets**-Liste, die Sie in der vorherigen Einheit konfiguriert haben, und klicken Sie anschließend zum Erstellen eines neuen Listenelements (Tweet) auf **Neu**.</span><span class="sxs-lookup"><span data-stu-id="36d92-106">In SharePoint, open the **ContosoTweets** list you configured in the previous unit, and then select **New** to create a new list item (tweet).</span></span> 

    ![Erstellen eines neuen Tweets in der SharePoint-Liste](../media/sharepoint-list-home.png)

2. <span data-ttu-id="36d92-108">Geben Sie die unten stehenden Werte ein, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="36d92-108">Enter the following values, and then select **Save**.</span></span>

    - <span data-ttu-id="36d92-109">Geben Sie bei **Titel** „Promotions“ ein.</span><span class="sxs-lookup"><span data-stu-id="36d92-109">For **Title**, enter "Promotions".</span></span>
    - <span data-ttu-id="36d92-110">Geben Sie bei **Tweetinhalt** „Entdecken Sie die neuesten Contoso-Fußböden #contosoentdecken“ ein.</span><span class="sxs-lookup"><span data-stu-id="36d92-110">For **TweetContent**, enter "Check out the new line of Contoso Flooring #ohsocontoso".</span></span> <span data-ttu-id="36d92-111">Beachten Sie, dass der Tweet einen Hashtag enthält.</span><span class="sxs-lookup"><span data-stu-id="36d92-111">Notice that the tweet contains a hashtag.</span></span>
    - <span data-ttu-id="36d92-112">Geben Sie bei **Tweetdatum** das heutige Datum ein.</span><span class="sxs-lookup"><span data-stu-id="36d92-112">For **TweetDate**, enter today's date.</span></span>

    ![Neues SharePoint-Element](../media/sharepoint-new-tweet.png)

## <a name="step-two-change-the-flow"></a><span data-ttu-id="36d92-114">Schritt 2: Ändern des Flows</span><span class="sxs-lookup"><span data-stu-id="36d92-114">Step two: Change the flow</span></span>
1. <span data-ttu-id="36d92-115">Klicken Sie in Microsoft Flow auf **Meine Flows**.</span><span class="sxs-lookup"><span data-stu-id="36d92-115">In Microsoft Flow, select **My flows**.</span></span> 
2. <span data-ttu-id="36d92-116">Wählen Sie den Flow **Listenelemente nach Genehmigung in Twitter posten** aus, den Sie in der vorherigen Einheit konfiguriert haben, und wählen Sie dann unter **Ausführungsverlauf** den ausgeführten Flow aus.</span><span class="sxs-lookup"><span data-stu-id="36d92-116">Select the **Post list items to Twitter after approval** flow you configured in the previous unit, and then, under **Run history**, select the running flow.</span></span>

    ![Ausführungsverlauf](../media/run-history.png)

3. <span data-ttu-id="36d92-118">Wählen Sie den Trigger **Wenn ein neues Element erstellt wird** aus.</span><span class="sxs-lookup"><span data-stu-id="36d92-118">Select the **When a new item is created** trigger.</span></span> <span data-ttu-id="36d92-119">Stellen Sie sicher, dass die Informationen für das erstellte Listenelement angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="36d92-119">Make sure that the information for the list item you just created is shown.</span></span>

    ![Flowtrigger](../media/approval-flow.png)

4. <span data-ttu-id="36d92-121">Öffnen Sie im Posteingang von Microsoft Outlook die automatisch gesendete E-Mail mit der Genehmigungsanforderung, und klicken Sie auf **Genehmigen**.</span><span class="sxs-lookup"><span data-stu-id="36d92-121">In Microsoft Outlook, open the automated approval mail in the inbox, and then select **Approve**.</span></span> 

    ![Outlook-Anforderung](../media/outlook-mail.png)

5. <span data-ttu-id="36d92-123">Sehen Sie sich die Details der Anforderung im Genehmigungscenter an, fügen Sie einen Kommentar hinzu, und klicken Sie anschließend auf **Bestätigen**.</span><span class="sxs-lookup"><span data-stu-id="36d92-123">In the Approval Center, view the details of the request, add a comment, and then select **Confirm**.</span></span> 

    ![Genehmigungscenter](../media/approval-center.png)

6. <span data-ttu-id="36d92-125">Aktualisieren Sie in SharePoint die **Contoso-Tweets**-Liste.</span><span class="sxs-lookup"><span data-stu-id="36d92-125">In SharePoint, refresh the **ContosoTweets** list.</span></span> <span data-ttu-id="36d92-126">Stellen Sie sicher, dass **Ja** als **Genehmigungsstatus** festgelegt ist und der eingegebene Kommentar angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="36d92-126">Make sure that **ApprovalStatus** is set to **Yes**, and that the comment you just entered is shown.</span></span> 

    ![Aktualisieren der SharePoint-Liste](../media/sharepoint-list-approved.png)

<span data-ttu-id="36d92-128">In dieser Einheit wurde beschrieben, wie der Vorgang aus der Perspektive der genehmigenden Person abläuft. Dabei wurden die Schritte vom Empfang der E-Mail mit der Genehmigungsanforderung bis zur Verarbeitung der Anforderung im Genehmigungscenter erläutert.</span><span class="sxs-lookup"><span data-stu-id="36d92-128">In this unit, you saw the experience from the approver's point of view, from receiving an approval request email to processing the request in the Approval Center.</span></span>