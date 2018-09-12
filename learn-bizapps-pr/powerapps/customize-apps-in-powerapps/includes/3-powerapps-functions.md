Wenn Sie Microsoft PowerApps verwenden, müssen Sie komplexe Anwendungen nicht auf die herkömmliche Weise programmieren. Weiterhin erforderlich ist jedoch, dass Sie Logik in einer App ausdrücken und die Navigation, Filterung, Sortierung und andere Funktionen einer App steuern. Hier kommen Formeln ins Spiel.

Wenn Sie schon einmal Microsoft Excel-Funktionen verwendet haben, sollte Ihnen der Ansatz von PowerApps vertraut vorkommen. In dieser Einheit werden einige einfache Formeln für die Textformatierung demonstriert. Anschließend werden drei Formeln vorgestellt, die PowerApps beim Erstellen einer App integriert. Sie erhalten einen Eindruck davon, was mit Formeln möglich ist, und schreiben außerdem Ihre eigenen.

## <a name="get-started-with-formulas-and-properties"></a>Erste Schritte mit Formeln und Eigenschaften
In der vorherigen Einheit wurden Steuerelemente auf allen drei Bildschirmen der App vorgestellt, die von PowerApps generiert wurde. In diesem Abschnitt wird der Preis formatiert, den Sie zuvor dem Bildschirm zum Durchsuchen hinzugefügt haben.

Der Preis wird standardmäßig als einfache Zahl ohne Währungssymbol angezeigt. Angenommen, Sie möchten ein Dollarzeichen hinzufügen und die Textfarbe abhängig vom Preis des Artikels ändern (z.B. Rot bei mehr als 5 $, andernfalls Grün). Auf der folgenden Abbildung wird das erwartete Ergebnis angezeigt.

![Textformatierung für Farbe und Währung](../media/conditional-format.png)

Beginnen wir mit der Währungsformatierung. Standardmäßig ruft PowerApps lediglich einen Preiswert für jedes Angebot ab. Dieser Wert wird als die **Text**-Eigenschaft der Beschriftung festgelegt, die den Preis anzeigt.

1. Wählen Sie auf dem Bildschirm **BrowseScreen1** den Preis des ersten Elements aus.

    ![Auswählen des Preises](../media/select-price.png)

1. Wählen Sie in der Dropdownliste mit den Eigenschaften **Text** aus.

    ![Preisformatierung](../media/powerapps-formulas1.png)

1. Legen Sie für die **Text**-Eigenschaft die folgende Formel fest, um das Währungssymbol für US-Dollar hinzuzufügen:

    `Text(Price, "[$-en-US]$ ##.00")`

Mit der **Text**-Funktion wird festgelegt, wie die Zahl formatiert werden soll. Diese Formel ist mit einer Excel-Funktion vergleichbar. PowerApps Formeln verweisen jedoch auf Steuerelemente und andere App-Elemente statt auf Zellen in einer Arbeitsmappe.

Wenn Sie ein Steuerelement auswählen und dann die Dropdownliste mit den Eigenschaften aufrufen, wird Ihnen eine Liste von Eigenschaften angezeigt, die für dieses Steuerelement relevant sind. Der folgende Listenausschnitt enthält einige der Eigenschaften für das **Beschriftungssteuerelement**. Manche Eigenschaften sind für eine Vielzahl von Steuerelementen relevant, während andere nur für ein spezifisches Steuerelement von Bedeutung sind.

![Festlegen von Eigenschaften](../media/powerapps-formulas4.png)

Legen Sie für die **Color**-Eigenschaft des **Preis-Beschriftungssteuerelements** die folgende Formel fest, um eine bedingte Formatierung der Farbe durchzuführen:

`If(Price > 5, Color.Red, Color.Green)`

## <a name="formulas-included-in-the-generated-app"></a>Formeln in der generierten App
Nachdem Sie nun gesehen haben, wie Formeln in Verbindung mit Eigenschaften verwendet werden, werden im Folgenden Beispiele für Formeln vorgestellt, die PowerApps in jeder generierten App verwendet. Beide Beispiele wurden bereits für den Bildschirm zum Durchsuchen verwendet und nutzen die **OnSelect**-Eigenschaft. Mit dieser Eigenschaft wird festgelegt, welche Aktion ausgeführt wird, wenn ein Benutzer ein Steuerelement auswählt (z.B. durch Klicken mit der Maus).

* Die erste Formel ist dem **IconNewItem1**-Steuerelement zugeordnet ![Symbol für neues Element](../media/powerapps-icon-add-item.png). Wenn Sie dieses Steuerelement auswählen, wird der Bildschirm zum Erstellen und Bearbeiten eines Elements geöffnet. Die Formel lautet wie folgt:

    `NewForm(EditForm1);Navigate(EditScreen1, ScreenTransition.None)`

    Die Formel instanziiert ein Bearbeitungsformular auf dem Bildschirm zum Bearbeiten und Erstellen eines Elements. Durch den Wert `ScreenTransition.None` wird angegeben, dass kein Übergang zwischen den Bildschirmen (beispielsweise durch Ausblenden) erfolgen soll.

* Die zweite Formel ist dem **IconSortUpDown1**-Steuerelement zugeordnet ![Sortiersymbol für Katalog](../media/powerapps-icon-sort.png). Wenn Sie dieses Steuerelement auswählen, werden die Elemente im Katalog sortiert. Die Formel lautet wie folgt:

    `UpdateContext({SortDescending1: !SortDescending1})`

    Die Formel verwendet `UpdateContext` zum Aktualisieren einer Variable mit der Bezeichnung `SortDescending1`. Der Wert der Variablen wechselt jeweils beim Klicken auf das Steuerelement. Mithilfe dieser Variable wird dem Katalog auf diesem Bildschirm mitgeteilt, wie die Elemente sortiert werden sollen.

Es gibt viele andere Formeln in der App, nehmen Sie sich also ein wenig Zeit, klicken Sie auf Steuerelemente und sehen sich an, welche Formeln für verschiedene Eigenschaften festgelegt wurden.

Weitere Informationen zu diesen und anderen Funktionen finden Sie in der [Referenz zu Formeln](https://docs.microsoft.com/powerapps/maker/canvas-apps/formula-reference).

## <a name="wrapping-it-all-up"></a>Zusammenfassung
Sie haben sich in dieser Einheit ausführlich mit der generierten App auseinandergesetzt und einen Blick auf Bildschirme, Steuerelemente, Eigenschaften und Formeln geworfen, die die Funktionen der App und deren individuelles Verhalten bestimmen. Wenn Sie die Vorgehensweise bis hierhin verfolgt haben, sollten Sie nun über ein tiefgreifenderes Verständnis der Funktionsweise einer generierten App verfügen. Sie können dieses Wissen nun anwenden, um Ihre eigene App zu erstellen.