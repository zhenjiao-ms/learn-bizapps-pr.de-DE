Diese Übung bringt Ihnen die Grundlagen von Dynamics 365 for Customer Service näher. Nach dem Absolvieren der Aufgaben in dieser Übung sind Sie auf einem guten Weg, Ihren Kunden zu helfen, Lösungen für Probleme mit Produkten und Diensten zu finden.

Für die folgenden Szenarien müssen Sie über eine Testumgebung oder eine vollwertige Instanz von [Customer Service](https://trials.dynamics.com/Dynamics365/Signup/service) verfügen.

Außerdem müssen Sie die Rolle „Kundenservicemanager“, die Rolle „Kundenservicemitarbeiter“ oder die entsprechenden Berechtigungen besitzen. [Finden Sie heraus, ob Sie über die erforderlichen Berechtigungen verfügen](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/basics/view-your-user-profile).

## <a name="scenario"></a>Szenario
Alle folgenden Szenarios basieren auf der folgenden Voraussetzung. HCL ist ein professionelles Dienstleistungsunternehmen. Die meisten seiner Gewinne stammen aus den Supportdiensten, die es seinen Kunden anbietet. HCL bietet den Kunden Helpdeskdienstleistungen während der normalen Geschäftszeiten von 8:00 bis 17:00 Uhr an. Für bevorzugte Kunden bietet es täglichen Support rund um die Uhr.

Bevorzugte Kunden werden in drei Stufen aufgeteilt:

- **Gold**: Diese Kunden genießen höchste Priorität. Sie erhalten garantiert eine Antwort innerhalb von 15 Minuten.
- **Silber**: Diese Kunden erhalten garantiert innerhalb einer Stunde einen Rückruf von einem Kundenservicemitarbeiter.
- **Bronze**: Diese Kunden haben Anspruch auf täglichen Support rund um die Uhr bei einer zweistündigen Antwortzeit.

HCL hat zwei Bereiche erkannt, auf die es seine Aufmerksamkeit richten möchte: 

- Jeder Kundenservicemitarbeiter sollte ein zentralisiertes Dashboard haben, das die täglichen Arbeitsauslastungen des Mitarbeiters anzeigt. Das Dashboard sollte die folgenden Informationen enthalten:

    - Eine Liste aller offenen Anfragen, die dem Kundenservicemitarbeiter derzeit zugewiesen sind
    - Eine Liste aller offenen Aktivitäten, die dem Mitarbeiter zugewiesen sind 
    - Anfragen nach Ursprung
    - Anfragen nach Priorität

- Mitarbeiter können Anfragen von neuen oder bestehenden Kunden übernehmen. Vor dem Erstellen einer Anfrage sollten Mitarbeiter einfach erkennen können, ob es sich um einen neuen oder einen bestehenden Kunden handelt:

    - Wenn es sich bei dem Kunden um einen Bestandskunden handelt, können die Mitarbeiter die Anfrage direkt erstellen.
    - Wenn es sich um einen neuen Kunden handelt, müssen Mitarbeiter erst einen neuen Datensatz für den Kunden erstellen. Sie können dann eine Anfrage für den Kunden erstellen.

### <a name="scenario-one-create-a-new-account"></a>Szenario eins: Ein neues Konto erstellen

Eine neue Kundin namens Paula Albrecht, die für Coho Consulting tätig ist, hat gerade bezüglich des folgenden Problems bei HCL angerufen:

- Bei einer Netzwerksicherung am vorherigen Abend ist ein Fehler aufgetreten. 

Auszuführende Aufgaben für dieses Szenario:

1. Fügen Sie ein neues Konto für Coho Consulting hinzu.
2. Fügen Sie einen Kontaktdatensatz für Paula Albrecht zu Coho Consulting hinzu.
3. Erstellen Sie eine neue Anfrage für Coho Consulting. Diese Anfrage enthält die folgenden Informationen:

**Neues Konto für Coho Consulting hinzufügen**

1. Wechseln Sie im Kundenservicezentrum zu **Service**, und wählen Sie dann **Konten** aus.
1. Wählen Sie auf der Befehlsleiste **Neu** aus.
1. Füllen Sie die Informationen über das Konto aus.
1. Wählen Sie **Speichern** aus.

   ![Neues Kundenkonto](../media/new-account.PNG)

**Fügen Sie einen Kontaktdatensatz für Paula Albrecht zu Coho Consulting hinzu.**

1. Suchen Sie die Tabelle **Kontakte**.
1. Wählen Sie das Pluszeichen (**+**) aus, um einen neuen Kontakt hinzuzufügen.
1. Tragen Sie die erforderlichen Kontaktinformationen ein.
1. Wählen Sie **Speichern** aus.

   ![Neuer Kontakt](../media/contacts.PNG)

**Neue Anfrage für Coho Consulting erstellen**

1. Gehen Sie zu **Service** &gt; **Anfragen**.
1. Wählen Sie **Neue Anfrage** aus.
1. Geben Sie für **Anfragentitel** *Fehler bei Netzwerksicherung* ein.
1. Für **Kunde** geben Sie *Coho Consulting* ein.
1. Für **Kontakt** geben Sie *Paula Albrecht* ein.
1. Für **Ursprung** geben Sie *Telefon* ein.
1. Für **Priorität** geben Sie *Hoch* ein.
1. Wählen Sie **Speichern** aus.

   ![Neue Anfrage](../media/cases.PNG)

### <a name="scenario-two-add-detail-to-a-case"></a>Szenario zwei: Einer Anfrage Details hinzufügen
HCL berechnet den Kunden die Gesamtzeit, die ein Agent mit einem Anruf verbringt. Die benötigte Gesamtzeit ist eine Zusammenfassung aller Aktivitäten, die einer bestimmten Anfrage zugeordnet sind. Agents müssen bei der Bearbeitung von Anrufen alle Aktivitäten im Zusammenhang mit einer Anfrage dokumentieren.

Nach einigen Recherchen stellt der Agent fest, dass das Problem des Kunden aufgetreten ist, weil der vorhergehende Tag ein Feiertag war. Aufgrund des Feiertags wurden die vorherigen Sicherungsmedien nicht ersetzt. Der Sicherungsauftrag überschreibt keine Medien, die in den letzten 48 Stunden bearbeitet wurden.

Da an diesem Tag keine Geschäfte getätigt wurden, kann der Agent den Sicherungsauftrag überspringen.

Auszuführende Aufgaben für dieses Szenario:

1. Fügen Sie eine Aufgabe für eine eingehende Telefonanrufaktivität von Paula Albrecht hinzu.
2. Fügen Sie der Anfrage eine Aufgabe hinzu, die vom Agent ausgeführt werden soll.
3. Fügen Sie der Aufgabe *Paula Albrecht über Lösung informieren* eine ausgehende Telefonanrufaktivität hinzu.

**Fügen Sie der Anfrage eine Aufgabe für eine eingehende Telefonanrufaktivität hinzu.**

1. Klicken Sie auf der Registerkarte **Aktivitäten** in der Mitte auf **Telefonanruf hinzufügen**.
1. Legen Sie die Dauer auf 15 Minuten fest.
1. Fügen Sie die folgende Notiz hinzu: *Erster Anruf von Paula Albrecht, die die Entdeckung einer fehlgeschlagenen Sicherung meldet*.
1. Wählen Sie **OK** aus.

**Der Anfrage eine Aufgabe hinzufügen, die vom Agent ausgeführt werden soll**

1. Wählen Sie auf der Registerkarte **Aktivitäten** die Auslassungspunkte (**…**) aus.
1. Wählen Sie **Aufgabe** aus. 
1. Legen Sie die Dauer auf 30 Minuten fest.
1. Fügen Sie den folgenden Hinweis hinzu: *Aufgrund eines Feiertags wurde das vorherige Sicherungsmedium nicht ausgetauscht. Die Sicherung überschreibt keine Medien, die in den vergangenen 48 Stunden geschrieben wurden*.
1. Wählen Sie **OK** aus. 

**Ausgehende Telefonanrufaktivität hinzufügen**

1. Suchen Sie **Aktivitäten**.
1. Wählen Sie **Telefonanruf hinzufügen** aus.
1. Legen Sie die Dauer auf 15 Minuten fest.
1. Fügen Sie die folgende Notiz hinzu: *Paula Albrecht angerufen, um sie über die Lösung zu informieren*.
1. Wählen Sie **OK** aus. 

### <a name="scenario-three-resolve-a-case"></a>Szenario drei: Eine Anfrage abschließen
Nach Abwicklung und Abschluss einer Anfrage muss der Agent die Anfrage abschließen. Zum Abschließen einer Anfrage müssen Agents ihre Aktivitäten im Zusammenhang mit der Anfrage notieren. Agents müssen auch die Zeit ausweisen, die sie mit Arbeit an den Anfrageaktivitäten verbracht haben.

Auszuführende Aufgaben für dieses Szenario:

1. Stellen Sie sicher, dass alle Aktivitäten im Zusammenhang mit der Anfrage abgeschlossen sind.
2. Schließen Sie die Anfrage ab.

**Alle Aktivitäten im Zusammenhang mit der Anfrage als abgeschlossen markieren**

1. Öffnen Sie jede Aktivität für die Anfrage. Stellen Sie sicher, dass alle Aktivitäten im Zusammenhang mit der Anfrage abgeschlossen sind.
1. Wählen Sie **Als abgeschlossen markieren** aus.

**Die Anfrage abschließen**

1. Klicken Sie auf der Befehlsleiste auf **Anfrage abschließen**.
1. Wählen Sie im Dialogfeld **Anfrage abschließen** in der Liste **Abschlusstyp** aus, wie die Anfrage abgeschlossen wurde. 
1. Geben Sie im Feld **Auflösung** eine kurze Erklärung zum Abschluss ein. 
1. Wählen Sie **Abschließen** aus.

### <a name="scenario-four-route-a-case"></a>Szenario vier: Eine Anfrage weiterleiten
HCL benötigt vier Warteschlangen, die zum Weiterleiten von Anfragen verwendet werden können, damit Agents daran arbeiten:

- Gold 
- Silber 
- Bronze 
- Standard 

Wenn eine neue Anfrage erstellt wird, muss das Servicelevel auf ihr vermerkt sein. Auf Grundlage des Servicelevels wird die Anfrage automatisch an die richtige Warteschlange weitergeleitet. Hier sehen Sie Regeln, die erstellt werden müssen, um die automatische Weiterleitung auszuführen: 

- Leiten Sie alle Anfragen mit Servicelevel Gold an die Warteschlange Gold weiter.
- Leiten Sie alle Anfragen mit Servicelevel Silber an die Warteschlange Silber weiter.
- Leiten Sie alle Anfragen mit Servicelevel Bronze an die Warteschlange Bronze weiter.
- Leiten Sie alle Anfragen ohne definiertes Servicelevel an die Warteschlange Standard weiter. 

Auszuführende Aufgaben für dieses Szenario:

1. Erstellen Sie die Warteschlangen.
2. Erstellen Sie die Regeln.

**Die Warteschlangen erstellen**

Erstellen Sie vier Warteschlangen in der Anwendung: Gold, Silber, Bronze und Standard.

1. Wechseln Sie zu **Einstellungen**, und wählen Sie dann **Serviceverwaltung** aus. 
   ![Einstellungen des Moduls "Serviceverwaltung"](../media/settings.PNG)
1. Wählen Sie **Warteschlangen** aus.
1. Wählen Sie **Neu** aus.
1. Geben Sie den Namen der ersten Warteschlange ein.
1. Wählen Sie **Speichern** aus.
1. Wiederholen Sie die Schritte 3 bis 5 für jede zusätzliche Warteschlange, die Sie erstellen müssen.

    ![Neue Warteschlange](../media/new-queue.PNG)


**Regeln erstellen**

Erstellen Sie Routingregeln, die Anfragen je nach deren Servicelevel an die entsprechenden Warteschlangen weiterleiten. 

1. Wechseln Sie zu **Einstellungen**, und wählen Sie dann **Serviceverwaltung** aus.
1. Wählen Sie **Routingregelsätze** aus.
1. Wählen Sie **Neu** aus. 
1. Wählen Sie **Regel für Anfragenweiterleitung** aus.
1. Wählen Sie **Speichern** aus. 
1. Wählen Sie im Abschnitt **Regelelemente** die Option **Regel hinzufügen**, um Bedingungen für die Weiterleitung von Anfragen an eine Warteschlange festzulegen. 
1. Geben Sie im Formular **Regelelement** einen beschreibenden Namen für das Regelelement ein. Geben Sie beispielsweise *Gold* ein.
1. Legen Sie unter **Regelkriterien** im Abschnitt **Wenn-Bedingungen** die Bedingungen fest, unter denen die Anfrage weitergeleitet wird. Beispiel: Legen Sie *Anfrage – Servicelevel – Gleich – Gold* fest.
1. Legen Sie unter **Dann-Bedingungen** die Warteschlange fest, an die die Anfrage weitergeleitet werden soll. Beispiel: Wählen Sie die Warteschlange **Gold** aus.
1. Wählen Sie **Speichern** und anschließend **Schließen** aus.
1. Wiederholen Sie die Schritte 6 bis 10 für jede zusätzliche Warteschlange, an die Sie Elemente weiterleiten müssen.
1. Wählen Sie im Datensatz **Routingregelsatz** die Option **Aktivieren** aus.

### <a name="scenario-five-manage-a-case"></a>Szenario fünf: Eine Anfrage verwalten

Dieses Szenario setzt das vorherige Szenario fort, indem die Aufgaben auf das Unternehmen Coho Consulting angewandt werden. Für dieses Szenario nehmen wir an, dass Coho Consulting gerade Gold-Kunde bei Ihrem Unternehmen geworden ist. Paula Albrecht hat HCL noch einmal angerufen. Sie hat ein Problem mit einem Drucker, der vor kurzem eingerichtet wurde.

Da es sich bei Coho Consulting um einen Gold-Kunden handelt, muss die erstellte Anfrage an die Gold-Warteschlange weitergeleitet werden.

Auszuführende Aufgaben für dieses Szenario:

1. Erstellen Sie die Anfrage.
2. Leiten Sie die Anfrage an die Gold-Warteschlange weiter.
3. Bearbeiten Sie die Anfrage.

**Erstellen einer Anfrage**

1. Wechseln Sie zu **Service**, und wählen Sie dann **Anfragen** aus.
1. Wählen Sie **Neue Anfrage** aus. 
1. Geben Sie als **Anfragentitel** *Druckerproblem* ein.
1. Für **Kunde** geben Sie *Coho Consulting* ein.
1. Für **Kontakt** geben Sie *Paula Albrecht* ein.
1. Für **Ursprung** geben Sie *Telefon* ein.
1. Für **Servicelevel** geben Sie *Gold* ein.
1. Wählen Sie **Speichern** aus.

**Die Anfrage an die Gold-Warteschlange weiterleiten**

- Wählen Sie auf der Befehlsleiste **Speichern** und dann **Weiterleiten** aus. 

**Die Anfrage bearbeiten**

Suchen Sie die Anfrage in der Gold-Warteschlange, und wählen Sie sie aus, damit Sie sie bearbeiten können.

1. Wechseln Sie zu **Service**, und wählen Sie dann **Warteschlangen** aus.
1. Wählen Sie eine Ansicht und einen Filter aus, um die gewünschten Elemente zu sehen.
1. Um alle Anfragen in der ausgewählten Warteschlange zu sehen, wählen Sie in der Liste **Ansicht** die Option **Alle Anfragen in ausgewählten Warteschlangen** aus.
1. Wählen Sie in der Liste **Warteschlange** die Warteschlange **Gold** aus.
1. Wählen Sie die Anfrage oder das Element zur Bearbeitung aus, und wählen Sie dann auf der Befehlsleiste die Option **Auswählen** aus.