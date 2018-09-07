In dieser Einheit erfahren Sie mehr über die Microsoft Flow-Umgebung, während Sie Ihren ersten Flow erstellen.

Es kann zeitaufwändig sein, in E-Mails nach Anhängen zu suchen. Der Flow, den Sie im Rahmen dieser Einheit erstellen, spart Zeit, indem all Ihre E-Mail-Anhänge in einem Ordner in Ihrem Microsoft OneDrive for Business-Konto gespeichert werden.

## <a name="choose-a-template"></a>Auswählen einer Vorlage
Mit vielen der Vorlagen können Sie im Handumdrehen Flows erstellen. Diese unterstützen Sie beim Verknüpfen der Dienste, die Sie bereits auf bedeutsameren Weisen verwenden.

Öffnen Sie die [Microsoft Flow-Website](https://ms.flow.microsoft.com), und wählen Sie das Menü **Vorlagen** aus. Wenn Sie durch die Liste scrollen, werden Sie bemerken, dass Microsoft Flow die Verknüpfung mit vielen Diensten ermöglicht.

Wählen Sie die Vorlage **Office 365-E-Mail-Anlagen in OneDrive for Business speichern** aus.

![Office 365-E-Mail](../media/office-365-email.png)

## <a name="create-the-flow"></a>Erstellen des Flows
**Office 365-E-Mail-Anlagen in OneDrive for Business speichern** ist eine One-Click-Vorlage, für die Sie nur Fragen beantworten, die zum Erstellen des Flows erforderlich sind, ohne auch nur eine Codezeile schreiben zu müssen.

Auf der Vorlagengrafik finden Sie eine Beschreibung der Funktionsweise der Vorlage und was erforderlich ist, damit sie erfolgreich ausgeführt wird.

Sie werden dazu aufgefordert, Anmeldeinformationen für die Microsoft Office 365 Outlook- und Microsoft SharePoint-Dienste anzugeben. Wenn Sie beide Dienste regelmäßig verwenden, werden Sie vermutlich bereits angemeldet sein.

1. Klicken Sie auf **Flow erstellen**.

    ![Speichern von Office 365-E-Mails](../media/save-flow-office-description.png)

    Flow erstellt einen Ordner auf Ihrem OneDrive for Business-Konto und speichert alle Anhänge, die an Ihre geschäftliche E-Mail-Adresse gesendet werden, in diesem Ordner.

    ![Erfolgreiche Erstellung](../media/create-successful.png)

2. Wählen Sie das Menü **Meine Flows** aus.

    ![Öffnen von „Meine Flows“](../media/click-my-flows.png)

3. Wählen Sie den soeben erstellten Flow aus, und machen Sie sich mit der Funktionsweise vertraut.

    ![Auswählen des Flows](../media/click-the-flow.png)

4. Ihnen wird ein grünes Häkchen angezeigt, das angibt, dass der Flow erfolgreich war. 
5. Klicken Sie auf **Bearbeiten**, um zu sehen, wie der Flow definiert wird.

    ![Aktionen bei neuen E-Mails](../media/trigger-or-action.png) 
 
6. Klicken Sie auf **Succeeded** (Erfolgreich), um den Ausführungsverlauf und die Ergebnisse anzuzeigen.

    ![Erfolgreicher Flow](../media/flow-successful.png)

    In diesem Fall waren alle Komponenten des Flows erfolgreich. 

    ![Ausführungsverlauf](../media/run-history.png)

## <a name="important-concepts-in-microsoft-flow"></a>Wichtige Konzepte in Microsoft Flow
Beachten Sie diese Konzepte beim Erstellen von Flows: 

- Jeder Flow enthält zwei Hauptkomponenten: einen *Auslöser* und mindestens eine *Aktion*.
- Sie können sich den Auslöser als Startaktion des Flows vorstellen. Der Auslöser kann eine neue E-Mail sein, die in Ihrem Posteingang ankommt, oder ein neues Element, das einer SharePoint-Liste hinzugefügt wird.
- Aktionen sollen ausgeführt werden, wenn ein Auslöser aufgerufen wird. Beispielsweise startet der Auslöser für neue E-Mails die Aktion zum Erstellen einer neuen Datei in OneDrive for Business. Zu anderen Beispielen für Aktionen gehört das Senden einer E-Mail, das Veröffentlichen eines Tweets und das Starten einer Genehmigung.

Diese Konzepte werden später aufgegriffen, wenn Sie Ihre eigenen Flows von Grund auf erstellen. 

In der nächsten Einheit erfahren Sie mehr über die Mobile App für Microsoft Flow und deren Funktionen. 
