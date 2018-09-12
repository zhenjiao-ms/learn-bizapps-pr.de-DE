In der vorherigen Einheit haben Sie erfahren, wie Sie einen Genehmigungsprozess für Tweets erstellen, die in einer Microsoft SharePoint-Liste gespeichert werden. In dieser Einheit wird beschrieben, was geschieht, wenn eine genehmigende Person eine neue Genehmigungsanforderung empfängt. 

## <a name="step-one-change-the-sharepoint-list"></a>Schritt 1: Anpassen der SharePoint-Liste
Zunächst fügen Sie Ihrer SharePoint-Liste ein Element hinzu. Anschließend kann eine Genehmigungsanforderung für dieses Element verarbeitet werden.

1. Öffnen Sie in SharePoint die **Contoso-Tweets**-Liste, die Sie in der vorherigen Einheit konfiguriert haben, und klicken Sie anschließend zum Erstellen eines neuen Listenelements (Tweet) auf **Neu**. 

    ![Erstellen eines neuen Tweets in der SharePoint-Liste](../media/sharepoint-list-home.png)

2. Geben Sie die unten stehenden Werte ein, und klicken Sie dann auf **Speichern**.

    - Geben Sie bei **Titel** „Promotions“ ein.
    - Geben Sie bei **Tweetinhalt** „Entdecken Sie die neuesten Contoso-Fußböden #contosoentdecken“ ein. Beachten Sie, dass der Tweet einen Hashtag enthält.
    - Geben Sie bei **Tweetdatum** das heutige Datum ein.

    ![Neues SharePoint-Element](../media/sharepoint-new-tweet.png)

## <a name="step-two-change-the-flow"></a>Schritt 2: Ändern des Flows
1. Klicken Sie in Microsoft Flow auf **Meine Flows**. 
2. Wählen Sie den Flow **Listenelemente nach Genehmigung in Twitter posten** aus, den Sie in der vorherigen Einheit konfiguriert haben, und wählen Sie dann unter **Ausführungsverlauf** den ausgeführten Flow aus.

    ![Ausführungsverlauf](../media/run-history.png)

3. Wählen Sie den Trigger **Wenn ein neues Element erstellt wird** aus. Stellen Sie sicher, dass die Informationen für das erstellte Listenelement angezeigt werden.

    ![Flowtrigger](../media/approval-flow.png)

4. Öffnen Sie im Posteingang von Microsoft Outlook die automatisch gesendete E-Mail mit der Genehmigungsanforderung, und klicken Sie auf **Genehmigen**. 

    ![Outlook-Anforderung](../media/outlook-mail.png)

5. Sehen Sie sich die Details der Anforderung im Genehmigungscenter an, fügen Sie einen Kommentar hinzu, und klicken Sie anschließend auf **Bestätigen**. 

    ![Genehmigungscenter](../media/approval-center.png)

6. Aktualisieren Sie in SharePoint die **Contoso-Tweets**-Liste. Stellen Sie sicher, dass **Ja** als **Genehmigungsstatus** festgelegt ist und der eingegebene Kommentar angezeigt wird. 

    ![Aktualisieren der SharePoint-Liste](../media/sharepoint-list-approved.png)

In dieser Einheit wurde beschrieben, wie der Vorgang aus der Perspektive der genehmigenden Person abläuft. Dabei wurden die Schritte vom Empfang der E-Mail mit der Genehmigungsanforderung bis zur Verarbeitung der Anforderung im Genehmigungscenter erläutert.