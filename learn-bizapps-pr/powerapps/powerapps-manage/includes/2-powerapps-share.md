Da Sie gelernt haben, wie Sie eine App erstellen, erfahren Sie nun, wie Sie sie freigeben. Sie können eine App für bestimmte Benutzer, Gruppen oder Ihre gesamte Organisation freigeben. Wenn Sie eine App für andere Personen freigeben, können diese sie von der Homepage von Microsoft Dynamics 365 in einem Webbrowser oder in Microsoft PowerApps Mobile für Microsoft Windows, Apple iOS oder Google Android ausführen.

Sie können sogar einer anderen Person die Berechtigung erteilen, die App zu aktualisieren.

## <a name="prepare-to-share-an-app"></a>Vorbereiten der Freigabe einer App

1. Klicken Sie in PowerApps Studio im Menü **Datei** auf **App-Einstellungen**.

1. Geben Sie einen aussagekräftigen Namen und eine Beschreibung für Ihre App ein, damit Ihr Team weiß, was Ihre App bewirkt, und sie leicht in einer Liste finden kann.

1. Wählen Sie im Menü **Datei** nacheinander **Speichern unter** und dann **Cloud** aus.

    Sie müssen eine App in der Cloud speichern, bevor Sie sie freigeben können.

1. Klicken Sie auf **Speichern** und dann auf **Diese App freigeben**.

1. Geben Sie auf der Registerkarte **Freigabe** an, für welche Benutzer oder Gruppen die App freigegeben werden soll. Klicken Sie auf die Schaltfläche **Alle Personen in meiner Organisation hinzufügen**, um alle Benutzer in Ihrer Organisation hinzuzufügen.

1. Aktivieren Sie das Kontrollkästchen **E-Mail-Einladung senden**, um Benutzer per E-Mail zu benachrichtigen.

    Wenn Sie dieses Kontrollkästchen aktivieren, erhält jede Person, für die Sie die App freigegeben haben, eine E-Mail-Nachricht mit einem Link zu Dynamics 365. Personen, denen Sie die Berechtigung zur Bearbeitung der App gewährt haben, erhalten auch einen Link zu „web.powerapps.com“.

    Die App wird nur den Personen angezeigt, die auf den Link zu Dynamics 365 klicken. Die App wird auch in Microsoft AppSource angezeigt. Jeder Benutzer, der nicht auf den Link geklickt hat, muss die App manuell aus AppSource in Dynamics 365 hinzufügen.

1. Geben Sie in der Liste **Freigegeben für** rechts in der Liste **Berechtigungen** an, wie die einzelnen Benutzer oder Gruppen mit der App interagieren können:

    - **Kann bearbeiten**: Benutzer können mit PowerApps Studio Änderungen an der App vornehmen.
    - **Kann verwenden**: Benutzer können die App anzeigen und verwenden, sie aber nicht ändern.

1. Klicken Sie auf **Speichern**.

Wenn Sie eine freigegebene App ändern und die Änderungen speichern, sind die Änderungen für die Personen, für die Sie die App freigegeben haben, nach dem Veröffentlichen der App sofort sichtbar. Diese direkte Verfügbarkeit kann zwar von Vorteil sein, wenn Sie die App verbessern, für andere Benutzer aber auch einen Nachteil bedeuten, wenn Sie Features entfernen oder erheblich ändern.

## <a name="permissions-and-licensing"></a>Berechtigungen und Lizenzierung

Im Folgenden finden Sie einige grundlegende Informationen zu Berechtigungen und Lizenzierung, die Sie kennen sollten:

- Benutzer und Mitwirkende benötigen Berechtigungen für alle Datenverbindungen und Gateways, die von einer freigegebenen App verwendet werden. Einige Berechtigungen werden implizit in der App gewährt, andere müssen von Ihnen jedoch explizit zugewiesen werden.
- Personen mit der Berechtigung **Kann bearbeiten** benötigen auch eine P2-Lizenz für PowerApps, um direkt mit Entitäten arbeiten zu können.

Das Freigeben von Apps ist ganz einfach und eine hervorragende Möglichkeit, eine App, die Sie hilfreich finden, für andere in Ihrer Organisation verfügbar zu machen.