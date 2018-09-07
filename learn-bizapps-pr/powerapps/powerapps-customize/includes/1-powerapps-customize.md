In einer vorherigen Einheit haben Sie die Flooring Estimates-App erstellt und sich mit ihrem Standarddesign vertraut gemacht. Von PowerApps generierte Standard-Apps sind nützlich. Häufig müssen Sie diese jedoch an Ihre eigenen Anforderungen anpassen.

In dieser Einheit erläutern wir einige einfache Änderungen, die für die einzelnen App-Bildschirme vorgenommen werden können. Es gibt zwar noch deutlich mehr Möglichkeiten zum Anpassen der App, doch für die ersten Schritte empfiehlt es sich, Anpassungen an einer generierten App vorzunehmen.

## <a name="browse-screen"></a>Bildschirm zum Durchsuchen
Wir beginnen mit dem Bildschirm zum Durchsuchen. In der App ist jedem Produkt bereits ein Bild und ein Text zugeordnet, doch das Layout könnte ansprechender gestaltet werden. Daran möchten wir jetzt arbeiten.

1. Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **BrowseGallery1**.

    Der Katalog wird daraufhin durch einen Rahmen hervorgehoben.

    ![Auswählen des Katalogs](../media/select-gallery.png)

1. Öffnen Sie im rechten Bereich den Bereich **Data** (Daten), indem Sie auf den Link neben **Layout** klicken.

    ![Anzeigen der Layoutoptionen](../media/powerapps-layout.png)

1. Wählen Sie ein anderes Layout aus, durch das z.B. das Bild, der Titel und der Untertitel werden, jedoch nicht der Text.

    ![Ändern des Layouts](../media/change-layout.png)

1. Wählen Sie im oberen Katalogbereich die Elementkategorie aus.

    ![Auswählen der Kategoriebeschriftung](../media/select-category.png)

1. Ändern Sie in der Formularleiste **ThisItem.Category** in **ThisItem.Name**.

1. Wiederholen Sie die vorherigen beiden Schritte, und passen Sie dabei das andere **Beschriftungssteuerelement** so an, dass für alle Elemente Preise angezeigt werden.

    ![Hinzufügen des Preises](../media/add-price.png)

Wie Sie sehen, können das Layout des Katalogs und die jeweiligen Datenkategorien ganz einfach angepasst werden. Vielleicht haben Sie sogar Spaß dabei.

## <a name="details-screen"></a>Detailbildschirm

Wir möchten die Reihenfolge der Felder auf dem Detailbildschirm ändern. Die Steuerelemente auf diesem Bildschirm unterscheiden sich von den Steuerelementen auf dem Bildschirm zum Durchsuchen. Daher gibt es auch leichte Abweichungen im Änderungsprozess.

1. Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **DetailForm1**.

1. Wählen Sie im rechten Bereich den Text aus, mit dem die Anzahl der ausgewählten Felder angezeigt wird.

    ![Auswählen des Texts, mit dem die Anzahl der ausgewählten Felder angezeigt wird](../media/powerapps-edit-fields.png)

1. Ziehen Sie das Feld **Name** in den oberen Bereich der Felderliste, und ziehen Sie das Feld **Image** (Bild) nach unten.

    ![Bewegen von Feldern auf dem Detailbildschirm](../media/powerapps-move-fields.png)

## <a name="editcreate-screen"></a>Bildschirm zum Erstellen/Bearbeiten

Abschließend soll nun auf dem Bildschirm, auf dem Benutzer Einträge erstellen und bearbeiten, die Eingabe von Informationen im Textfeld erleichtert werden.

1. Klicken Sie im linken Bereich **Screens** (Bildschirme) auf **EditForm1**.

1. Wählen Sie im rechten Bereich den Text aus, mit dem die Anzahl der ausgewählten Felder angezeigt wird.

1. Klicken Sie zuerst auf den Dropdownpfeil der Liste **Overview** (Übersicht) und anschließend auf **Mehrzeiligen Text bearbeiten**.

    Mit dem Bearbeitungssteuerelement für mehrzeiligen Text wird die Eingabe längerer Texte vereinfacht.

    ![Ändern von Feldern für den Bildschirm zum Erstellen/Bearbeiten](../media/powerapps-change-editscreen.png)

Nun wissen Sie, wie die Darstellung und Benutzerfreundlichkeit einer erstellten App mit einigen grundlegenden Schritten erheblich verbessert werden kann. In dieser Einheit haben Sie sich auf die Anwendung PowerApps Studio konzentriert, die viele Optionen zum Anpassen von Apps bereitstellt. In der nächsten Einheit werden die Steuerelemente der App ausführlicher dargestellt.