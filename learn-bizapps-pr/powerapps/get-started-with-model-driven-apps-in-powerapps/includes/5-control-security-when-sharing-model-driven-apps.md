Microsoft PowerApps verwendet rollenbasierte Sicherheit für die Freigabe. Eine Sicherheitsrolle enthält Berechtigungen, die eine Reihe von Aktionen definieren, die in der App ausgeführt werden können. Alle App-Benutzer müssen einer oder mehreren vordefinierten oder benutzerdefinierten Sicherheitsrollen zugewiesen werden.

Rollen können einzelnen Benutzern oder Teams zugewiesen werden. Wenn ein Benutzer oder Team einer Rolle zugewiesen wird, wird dem Benutzer oder allen Mitgliedern dieses Teams der Satz von Berechtigungen gewährt, die der Rolle zugeordnet sind.

In dieser Einheit erfahren Sie, wie Sie eine modellgesteuerte App freigeben, damit andere sie verwenden können.

Insbesondere erfahren Sie, wie Sie:

- Eine benutzerdefinierte Sicherheitsrolle erstellen.
- Benutzer der benutzerdefinierten Sicherheitsrolle zuweisen.
- Die Sicherheitsrolle einer App zuweisen.

Eine App können Sie nur in der Rolle des Umgebungsadministrators oder Systemadministrators freigeben.

## <a name="scenario"></a>Szenario
In dieser Einheit wird das Beispiel eines Unternehmens namens Contoso verwendet, das einen Geschäftsbereich Fellpflege für Hunde und Katzen betreibt. Eine App, die über eine benutzerdefinierte Entität zum Nachverfolgen des Geschäftsbereichs Fellpflege verfügt, wurde bereits erstellt und veröffentlicht.

Die App muss freigegeben werden, sodass das Fellpflegepersonal sie verwenden kann. Zum Freigeben der App weist ein Administrator oder App-Ersteller Benutzern und der App eine oder mehrere Sicherheitsrollen zu.

## <a name="create-or-set-up-a-security-role"></a>Erstellen oder Einrichten einer Sicherheitsrolle
Die PowerApps-Umgebung enthält vordefinierte Sicherheitsrollen. Diese Rollen entsprechen häufig verwendeten Benutzeraufgaben, und die Zugriffsebenen sind gemäß der bewährten Sicherheitsmethode zur Gewährung des Zugriffs auf die zur Verwendung der App erforderlichen Mindestmenge an Geschäftsdaten definiert.

Denken Sie daran, dass die Contoso-Fellpflege-App auf einer benutzerdefinierten Entität basiert. Da die Entität benutzerdefiniert ist, müssen Berechtigungen explizit angegeben werden, bevor Benutzer darin arbeiten können. Sie können hierzu einen der folgenden Ansätze verwenden:

- Erweitern Sie eine bereits vorhandene vordefinierte Sicherheitsrolle, sodass sie Berechtigungen für Datensätze enthält, die auf der benutzerdefinierten Entität basieren.
- Erstellen Sie eine benutzerdefinierte Sicherheitsrolle zum Verwalten von Berechtigungen für Benutzer der App.

Da die Umgebung, die die Fellpflegedatensätze verwaltet, auch für andere Apps verwendet wird, die das Unternehmen Contoso ausführt, wird eine spezifische benutzerdefinierte Sicherheitsrolle für die Fellpflege-App erstellt. Darüber hinaus sind zwei verschiedene Sätze von Zugriffsberechtigungen erforderlich:

- Haustierfriseure müssen nur Datensätze lesen, aktualisieren und andere Datensätze anfügen. Daher verfügt ihre Sicherheitsrolle über die Berechtigungen Lesen, Schreiben und Anfügen.
- Haustierpflegemanager benötigen alle Berechtigungen, über die Haustierfriseure verfügen. Darüber hinaus müssen sie Datensätze erstellen, anfügen an, löschen und freigeben. Darum verfügt ihre Sicherheitsrolle über Berechtigungen zum Erstellen, Lesen, Schreiben, Anfügen, Löschen, Zuweisen, Anfügen an und Freigeben.

Weitere Informationen zu Zugriff und Bereich der verschiedenen Berechtigungen finden Sie unter [Sicherheitsrollen](https://docs.microsoft.com/dynamics365/customer-engagement/admin/security-roles-privileges#security-roles).

## <a name="create-a-custom-security-role"></a>Erstellen einer benutzerdefinierten Sicherheitsrolle
1. Melden Sie sich mit Ihrem Unternehmenskonto bei [PowerApps](https://powerapps.microsoft.com/) an. Wenn Sie noch nicht über ein Konto verfügen, wählen Sie **Kostenlos beginnen** aus.
1. Wählen Sie auf der PowerApps-Startseite **Modellgesteuert** aus.
1. Klicken Sie für Ihre neue App zuerst auf die Schaltfläche **Weitere Befehle** (**...**) und anschließend auf **Freigeben**.
1. Klicken Sie im Dialogfeld **Diese App freigeben** unter **Sicherheitsrolle erstellen** auf den Link **Sicherheitseinstellung**.
1. Klicken Sie auf der Seite **Alle Rollen** auf **Neu**.
1. Geben Sie im Feld **Rollenname** die Bezeichnung *Pet Grooming Technicians* (Haustierpflege-Fachkräfte) ein.
1. Suchen Sie im Sicherheitsrollen-Designer auf der Registerkarte **Benutzerdefinierte Entitäten** die Entität **Pet** (Haustier).
1. Klicken Sie in der Zeile **Pet** viermal auf **Lesen**, **Schreiben** und **Anfügen**, um den *Organisationsbereich* jeweils auf ![Global organization scope](../media/organizational-scope-privilege.png) (Globaler Organisationsbereich) festzulegen.

    ![Neue Sicherheitsrolle](../media/custom-security-role.png)

1. Die Haustierpflege-App hat auch eine Beziehung zur Kontoentität. Klicken Sie auf der Registerkarte **Core Records** (Kerndatensätze) in der Zeile **Konto** viermal auf die Berechtigung **Lesen**, bis sie auf den *Organisationsbereich* ![Global organization scope](../media/organizational-scope-privilege.png) (Globaler Organisationsbereich) festgelegt wird. 
1. Klicken Sie auf **Speichern und ausführen**. 
1. Geben Sie im Sicherheitsrollen-Designer im Feld **Rollenname** die Bezeichnung *Pet Grooming Schedulers* (Personal für Planung von Haustierpflegeterminen) ein. 
1. Suchen Sie auf der Registerkarte **Benutzerdefinierte Entitäten** nach der Entität **Pet**. 
1. Klicken Sie in der Zeile **Pet** viermal auf jede der folgenden Berechtigungen, bis der globale *Organisationsbereich* ![Global organization scope](../media/organizational-scope-privilege.png) (Globaler Organisationsbereich) ausgewählt wird: **Erstellen**, **Lesen**, **Schreiben**, **Löschen**, **Anfügen**, **Anfügen an**, **Zuweisen** und **Freigeben**.
1. Die Haustierpflege-App hat auch eine Beziehung zur Kontoentität, und das Personal für die Terminplanung muss Kontodatensätze erstellen und ändern können. Klicken Sie darum auf der Registerkarte **Core Records** (Kerndatensätze) in der Zeile **Konto** viermal auf jede der folgenden Berechtigungen, bis der *Organisationsbereich* ![Global organization scope](../media/organizational-scope-privilege.png) (Globaler Organisationsbereich) ausgewählt wird: **Erstellen**, **Lesen**, **Schreiben**, **Löschen**, **Anfügen**, **Anfügen an**, **Zuweisen** und **Freigeben**.
1. Wählen Sie **Speichern und Schließen** aus.

## <a name="assign-security-roles-to-users"></a>Zuweisen von Sicherheitsrollen an Benutzer
Sicherheitsrollen steuern den Benutzerzugriff auf Daten über mehrere Zugriffsebenen und Berechtigungen. Die Kombination von Zugriffsebenen und Berechtigungen, die in einer bestimmten Sicherheitsrolle enthalten sind, begrenzt die Datenansicht des Benutzers und seine Interaktionen mit den Daten.

### <a name="assign-a-security-role-to-the-pet-grooming-technicians"></a>Zuweisen einer Sicherheitsrolle für Haustierpflege-Fachkräfte
1. Wählen Sie im Dialogfeld **Diese App freigeben** unter **Der Sicherheitsrolle Benutzer zuweisen** die Option **Sicherheitsbenutzer** aus.
2. Wählen Sie in der angezeigten Liste die Haustierfriseure aus.
3. Wählen Sie **Rollen verwalten** aus.

    ![Verwalten von Rollen](../media/select-users-for-security-roles.png)

4. Wählen Sie im Dialogfeld **Benutzerrollen verwalten** die Sicherheitsrolle **Pet Grooming Technicians**, die Sie zuvor erstellt haben, und dann **OK** aus.

### <a name="assign-a-security-role-to-the-pet-grooming-schedulers"></a>Zuweisen einer Sicherheitsrolle für die Haustierpflegemanager
1. Wählen Sie im Dialogfeld **Diese App freigeben** unter **Der Sicherheitsrolle Benutzer zuweisen** die Option **Sicherheitsbenutzer** aus.
2. Wählen Sie in der angezeigten Liste die Haustierpflegemanager aus.
3. Wählen Sie **Rollen verwalten** aus.
4. Wählen Sie im Dialogfeld **Benutzerrollen verwalten** die Sicherheitsrolle **Pet Grooming Schedulers**, die Sie zuvor erstellt haben, und dann **OK** aus.

## <a name="add-security-roles-to-the-app"></a>Zuweisen von Sicherheitsrollen an die App
Als Nächstes müssen Sie der App eine oder mehrere Sicherheitsrollen zuweisen. Welche Apps Benutzer verwenden können, hängt von den Sicherheitsrollen ab, denen sie zugeordnet sind.

1. Wählen Sie im Dialogfeld **Diese App freigeben** unter **Ihrer App die Sicherheitsrolle hinzufügen** die Option **Meine Apps** aus.
2. Klicken Sie auf der Kachel für die Haustierpflege-App auf die Schaltfläche **Weitere Optionen** (**...** ) und anschließend auf **Rollen verwalten**.

    ![Verwalten von Rollen für die App](../media/manage-roles.png)

3. Im Abschnitt **Rollen** können Sie auswählen, ob Sie den Zugriff auf die App allen Sicherheitsrollen oder nur ausgewählten Rollen gewähren möchten. Wählen Sie die Rollen **Pet Grooming Schedulers** und **Pet Grooming Technicians** aus, die Sie zuvor erstellt haben.

    ![Auswählen der Sicherheitsrollen für die App](../media/app-security-roles.png)

4. Klicken Sie auf **Speichern**.

## <a name="share-the-link-to-your-app"></a>Freigeben des Links zu Ihrer App
1. Kopieren Sie im Dialogfeld **Diese App freigeben** unter **Den Link zu Ihrer App direkt mit Benutzern teilen** die angezeigte URL.
1. Klicken Sie auf **Schließen**.
1. Fügen Sie die URL in einen Speicherort ein, wo Ihre Benutzer darauf zugreifen können. Beispielsweise können Sie die URL auf einer Microsoft SharePoint-Website veröffentlichen oder per E-Mail senden.

Sie finden die URL der App auch im App-Designer auf der Registerkarte **Eigenschaften**.

![Kopieren der App-URL](../media/app-designer-copy-web-url.png)

## <a name="about-predefined-security-roles"></a>Informationen zu vordefinierten Sicherheitsrollen
Die folgenden vordefinierten Rollen sind mit einer PowerApps-Umgebung verfügbar. Sofern nicht anders angegeben, haben alle Berechtigungen globalen Gültigkeitsbereich.

| Sicherheitsrolle            | Rechte | Beschreibung |
|--------------------------|------------|-------------|
| Umgebungsersteller        | Keine | Benutzer mit dieser Rolle können neue Ressourcen erstellen, die einer Umgebung zugeordnet sind, einschließlich Apps, Verbindungen, benutzerdefinierter Anwendungsprogrammierschnittstellen (APIs), Gateways und Flows, die Microsoft Flow verwenden. Diese Benutzer können jedoch nicht auf die Daten in einer Umgebung zugreifen. Weitere Informationen zu Umgebungen finden Sie unter [Announcing PowerApps environments (Ankündigung: Umgebungen in PowerApps)](https://powerapps.microsoft.com/blog/powerapps-environments/). |
| Systemadministrator     | Erstellen, Lesen, Schreiben, Löschen, Anpassen | Diese Rolle verfügt über umfassende Berechtigungen zum Anpassen oder Verwalten der Umgebung, einschließlich Erstellen, Ändern und Zuweisen von Sicherheitsrollen. Benutzer mit dieser Rolle können alle Daten in der Umgebung anzeigen. Weitere Informationen finden Sie unter [Erforderliche Berechtigungen für Anpassungen](https://docs.microsoft.com/dynamics365/customer-engagement/customize/privileges-required-customization). |
| Systemanpasser        | Erstellen (selbst), Lesen (selbst), Schreiben (selbst), Löschen (selbst), Anpassungen | Diese Rolle verfügt über die volle Berechtigung zum Anpassen der Umgebung. Aber Benutzer mit dieser Rolle können Datensätze nur für Umgebungsentitäten anzeigen, die sie erstellen. Weitere Informationen finden Sie unter [Erforderliche Berechtigungen für Anpassungen](https://docs.microsoft.com/dynamics365/customer-engagement/customize/privileges-required-customization). |
| Common Data Service-Benutzer | Lesen, Erstellen (selbst), Schreiben (selbst), Löschen (selbst) | Benutzer mit dieser Rolle können eine App in der Umgebung und allgemeine Aufgaben für die Datensätze, die sie besitzen, ausführen. |
| Delegieren                 | Agieren im Auftrag eines anderen Benutzers | Diese Rolle kann Code als anderer Benutzer ausführen oder die Identität eines anderen Benutzers annehmen. Diese Rolle wird in der Regel mit einer anderen Sicherheitsrolle verwendet, um den Zugriff auf Datensätze bereitzustellen. Weitere Informationen finden Sie unter [Annehmen der Identität eines anderen Benutzers](https://docs.microsoft.com/dynamics365/customer-engagement/developer/org-service/impersonate-another-user). |
