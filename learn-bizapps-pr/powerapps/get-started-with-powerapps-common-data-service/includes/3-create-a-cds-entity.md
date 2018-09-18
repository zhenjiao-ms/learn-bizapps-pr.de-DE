In dieser Lektion erstellen Sie eine Entität und passen anschließend wichtige Komponenten wie Felder, Beziehungen, Ansichten und Formulare an. Sie lernen Folgendes:

- Erstellen einer benutzerdefinierten Entität
- Hinzufügen benutzerdefinierter Felder zur Entität
- Hinzufügen einer Entitätsbeziehung
- Anpassen einer Ansicht
- Anpassen eines Formulars

Dieses Tutorial orientiert sich am Unternehmen Contoso, das einen Haustierpflegedienst für Hunde und Katzen betreibt. Contoso benötigt eine App zum Nachverfolgen von Kunden und Haustieren, die von den Mitarbeitern auf einer Vielzahl von Geräten genutzt werden kann.

## <a name="prerequisites"></a>Voraussetzungen

Melden Sie sich bei [Microsoft PowerApps](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) an. Wenn Sie nicht bereits über ein PowerApps-Konto verfügen, klicken Sie auf [powerapps.com](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) auf den Link **Steigen Sie kostenlos ein**.

## <a name="create-a-custom-entity"></a>Erstellen einer benutzerdefinierten Entität

1. Erweitern Sie im linken Navigationsbereich **Daten**. Wählen Sie **Entitäten** und dann **Neue Entität** erstellen aus.

    > [!div class="mx-imgBorder"]
    > ![Neue Entität](../media/create-new-entity.png)

2. Geben Sie die folgenden Werte ein:

    - **Anzeigename**: *Haustier*
    - **Beschreibung**: *Benutzerdefinierte Entität zum Nachverfolgen von Dienstleistungen für Haustiere*

3. Klicken Sie auf **Weiter**, und wählen Sie dann, nachdem die Standardfelder eingeblendet wurden, **Entität speichern** aus.

## <a name="add-and-customize-fields"></a>Hinzufügen und Anpassen von Feldern

1. Wählen Sie in der Liste der Entitäten die Entität **Haustier** aus, die Sie im vorherigen Abschnitt erstellt haben.
2. Wählen Sie auf der Registerkarte **Felder** das Feld **Haustier** aus.
3. Nehmen Sie im rechten Bereich folgende Änderungen am Feld **Anzeigename** vor:

    - Ändern Sie den Wert **Anzeigename** von *Haustier* in *Name des Haustiers*.
    - Aktivieren Sie das Kontrollkästchen **Durchsuchbar**.

    > [!div class="mx-imgBorder"]
    > ![Primäres Feld ändern](../media/primary-field.png)

3. Klicken Sie auf **Fertig**.
4. Klicken Sie auf der Registerkarte **Felder** auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.
5. Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein:

    - **Anzeigename**: *Art*
    - **Datentyp**: *Optionssatz*
    - **Optionssatz**: *Neuer Optionssatz*

6. Erstellen Sie den Optionssatz:

    1. Klicken Sie auf **Neues Element hinzufügen**.
    2. Ersetzen Sie *Neue Option* durch *Hund*.
    3. Klicken Sie auf **Neues Element hinzufügen**.
    4. Ersetzen Sie *Neue Option* durch *Katze*.
    5. Klicken Sie auf **Speichern**.

    > [!div class="mx-imgBorder"]
    > ![Neuer Optionssatz](../media/optionset-add-items.png)

7. Aktivieren Sie **Durchsuchbar**, und klicken Sie dann auf **Fertig**.
8. Klicken auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.
9. Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein, und klicken Sie dann auf **Fertig**:

    - **Anzeigename**: *Rasse*
    - **Datentyp**: *Text*
    - **Durchsuchbar**: *Ja*

10. Klicken auf der Entity Designer-Symbolleiste auf **Feld hinzufügen**.
11. Geben Sie im Bereich **Feldeigenschaften** die folgenden Werte ein, und klicken Sie dann auf **Fertig**:

    - **Anzeigename**: *Datum des Termins*
    - **Datentyp**: *Datum und Uhrzeit*

12. Klicken Sie auf **Entität speichern**.

## <a name="add-a-relationship"></a>Hinzufügen einer Beziehung

1. Klicken Sie auf der Registerkarte **Beziehungen** auf der Entity Designer-Symbolleiste auf **Beziehung hinzufügen**, und wählen Sie dann **n:1** aus.
2. Wählen Sie im rechten Bereich in der Liste **Verknüpft** den Eintrag **Konto** aus.
3. Klicken Sie auf **Fertig**.
4. Klicken Sie auf **Entität speichern**.

    Beachten Sie, dass beim Hinzufügen einer n-:1-Beziehung ein Feld des Typs **Konto** mit dem Datentyp **Suche** automatisch zu Ihrer Liste der Felder auf der Registerkarte **Felder** hinzugefügt wird.

    > [!div class="mx-imgBorder"]
    > ![Feld zum Suchen eines Kontos](../media/account-lookup-field.png)

## <a name="customize-a-view"></a>Anpassen einer Ansicht

1. Wählen Sie auf der Registerkarte **Ansichten** die Ansicht **Aktive Haustiere** aus. Wenn die Ansicht **Aktive Haustiere** nicht angezeigt wird, wählen **Filter entfernen** aus.
2. Wählen Sie im Ansicht-Designer **Spalten hinzufügen** und dann die folgenden Spalten aus. Klicken Sie anschließend auf **OK**:

    - Konto
    - Datum des Termins
    - Rasse
    - Art

3. Klicken Sie auf die Spalte **Erstellt am**, dann auf **Entfernen** und anschließend auf **OK**, um das Entfernen der Spalte zu bestätigen.
4. Um die Spalten anzuordnen, wählen Sie die zu verschiebende Spalte aus, und klicken Sie dann auf die Pfeiltasten (**\<-** und **-\>**), bis Ihre Ansicht so aussieht.

    > [!div class="mx-imgBorder"]
    > ![Ansicht „Aktive Haustiere“](../media/active-pets-view.png)

5. Klicken Sie auf der Symbolleiste des Ansicht-Designers auf **Speichern und schließen**.

## <a name="customize-the-main-form"></a>Anpassen des Hauptformulars

1. Wählen Sie in PowerApps im linken Navigationsbereich **Modellgesteuert** aus.
2. Erweitern Sie im linken Navigationsbereich **Daten**. Wählen Sie **Entitäten** und dann **Haustier** aus.
3. Wählen Sie auf der Registerkarte **Formulare** den Eintrag **Informationen** neben dem Typ **Hauptformular** aus, um den Formular-Editor zu öffnen.

    > [!div class="mx-imgBorder"]
    > ![Bearbeiten des Hauptformulars](../media/main-form-edit.png)

4. Ziehen Sie im Formular-Editor die Felder **Art**, **Rasse**, **Datum des Termins** und **Konto** aus dem Bereich **Feld-Explorer** in den Abschnitt **Allgemein** des Formularzeichenbereichs, bis das Formular so aussieht.

    > [!div class="mx-imgBorder"]
    > ![Auswählen von Feldern für das Hauptformular](../media/main-form-edit2.png)

5. Klicken Sie auf **Speichern**.
6. Klicken Sie auf **Veröffentlichen**.
7. Klicken Sie auf **Speichern und schließen**, um den Formulardesigner zu schließen.
