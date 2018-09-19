Kommen wir jetzt zu den ersten Schritten.

Da Sie nun die Komponenten von Microsoft PowerApps und die Optionen zum Erstellen von Apps kennen, wird es Zeit, eine eigene App zu erstellen. In dieser Einheit erstellen Sie eine Smartphone-App, deren Datenquelle eine in Microsoft OneDrive for Business gespeicherte Microsoft Excel-Arbeitsmappe ist. In dieser Excel-Arbeitsmappe werden die Muster von Bodenbelägen eines Unternehmens einschließlich der zugehörigen Bilder und Preise aufgeführt.

Denken Sie daran, dass Sie auch Daten aus verschiedenen anderen Quellen verwenden können, z.B. aus Microsoft SharePoint, Clouddiensten wie Salesforce und lokalen Quellen wie Microsoft SQL Server.

## <a name="connect-to-a-data-source"></a>Herstellen einer Verbindung mit einer Datenquelle

1. Laden Sie die Arbeitsmappe [Flooring Estimates](https://az787822.vo.msecnd.net/documentation/get-started-from-data/FlooringEstimates.xlsx) herunter, und speichern Sie sie in OneDrive for Business.

1. Navigieren Sie zu [https://web.powerapps.com](https://web.powerapps.com), und melden Sie sich mit Ihrem Organisationskonto an.

1. Klicken Sie im linken Bereich auf die Option **Apps**.

1. Klicken Sie auf **Create an app** (App erstellen).

1. Klicken Sie für die Datenquelle **OneDrive for Business** auf **Telefonlayout**.

    ![Smartphone-App aus SharePoint-Liste](../media/powerapps-start-excel.png)

    Generierte Apps basieren immer auf einer einzelnen Liste oder Tabelle, aber Sie können der App später weitere Daten hinzufügen. Die nächsten drei Schritte erläutern, wie Sie eine Verbindung mit der Excel-Arbeitsmappe herstellen.

1. Wählen Sie unter **Verbindungen** die Option **OneDrive for Business** aus.
1. Wählen Sie unter **Choose an Excel file** (Excel-Datei auswählen) die Excel-Arbeitsmappe aus.
1. Klicken Sie auf **Verbinden**.

Zum Generieren der App untersucht PowerApps Ihre Daten und gleicht sie mit den PowerApps-Funktionen ab, sodass Sie eine funktionierende App als Ausgangspunkt erhalten.

## <a name="explore-the-generated-app"></a>Komponenten der generierten App
Vorgang erfolgreich! Ihre neue App mit drei Bildschirmen öffnet sich in PowerApps Studio.

Auf der linken Seite wird der Bereich **Bildschirme** angezeigt. Wählen Sie in der oberen rechten Ecke des Bereichs „Bildschirme“ die Miniaturansicht aus.

![Umschalten zwischen den Ansichten](../media/Powerapps-app-nav.png)

Wählen Sie für jeden Bildschirm die Miniaturansicht aus, um die Steuerelemente des jeweiligen Bildschirms anzuzeigen. 

Hier sehen Sie das Hauptentwicklungsfenster in PowerApps Studio, zu dem Sie in späteren Einheiten weitere Informationen erhalten.

![Die generierte App](../media/powerapps-full-screen2.png)

Klicken Sie in der oberen rechten Ecke auf **Wiedergeben** ![Pfeil zum Starten der App-Vorschau](../media/powerapps-arrow.png), um die App auszuprobieren. Wie Sie sehen, enthält die App alle Daten aus der Liste und ist in der Standardversion bereits gut zu bedienen.

Alle aus Daten generierten Apps verfügen über dieselben Bildschirme, die Sie im Miniaturansichtbereich anzeigen können:

* **Bildschirm zum Durchsuchen**: Dieser Bildschirm wird standardmäßig angezeigt. Hier können Sie die Daten aus Ihrer Datenquelle durchsuchen, sortieren, filtern und aktualisieren. In diesem Bildschirm können Sie Elemente zur Datenquelle hinzufügen, indem Sie auf das Pluszeichen klicken (**+**).
* **Bildschirm mit Details**: Wählen Sie im Bildschirm zum Durchsuchen ein Element aus, um den Detailbildschirm zu öffnen, in dem alle Details zu einem Element angezeigt werden. In diesem Bildschirm können Sie ein Element zum Bearbeiten öffnen oder ein Element löschen.
* **Bildschirm zum Bearbeiten/Erstellen**: in diesem Bildschirm bearbeiten Sie ein vorhandenes Element oder erstellen ein neues Element.

## <a name="install-the-app-on-your-device"></a>Installieren der App auf Ihrem Gerät
Sie sollten die App auf Ihrem Smartphone installieren, um sie zu testen.

1. Laden Sie PowerApps Mobile aus dem App-Store für die Plattform herunter, die Sie verwenden möchten.

2. Melden Sie sich mit Ihrem Benutzernamen und dem zugehörigen Kennwort an.

3. Wenn Sie auf dem Smartphone oder Tablet arbeiten, führen Sie die App zur Berechnung von Kostenvoranschlägen für Bodenbeläge (Flooring Estimates) in PowerApps Mobile aus. Andernfalls führen Sie die App in einem Browser aus.

Sie haben innerhalb weniger Minuten gelernt, wie Sie eine Verbindung mit einer Datenquelle herstellen und eine App generieren. Sie haben sich auch mit PowerApps Studio und den drei Bildschirmen in einer generierten App vertraut gemacht. In späteren Modulen erfahren Sie, wie Sie generierte Apps anpassen können.