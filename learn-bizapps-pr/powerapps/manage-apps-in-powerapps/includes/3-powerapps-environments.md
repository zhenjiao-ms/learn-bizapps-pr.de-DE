Eine Umgebung ist ein Container für Apps und andere Ressourcen wie Datenverbindungen und Flows aus Microsoft Flow. Sie stellt eine Möglichkeit dar, Elemente auf Grundlage Ihrer Geschäftsanforderungen zu gruppieren.

![Umgebungsauswahl](../media/powerapps-environments2.png)

Wenn Sie dieses Modul bis hierhin gelesen haben, haben Sie bereits einige Zeit auf https://web.powerapps.com gearbeitet. Bewusst oder unbewusst haben Sie dabei die ganze Zeit in einer Umgebung gearbeitet.

In der oberen rechten Ecke der Homepage von „web.powerapps.com“ können Sie sehen, in welcher Umgebung Sie sich aktuell befinden.

![Umgebungsauswahl](../media/powerapps-environment-picker.png)

Wenn Sie noch nicht viel mit Microsoft PowerApps gearbeitet haben, wird hier vermutlich nur die Standardumgebung angezeigt.

- Öffnen Sie das Menü, um zu sehen, ob andere Umgebungen verfügbar sind.

## <a name="why-use-environments"></a>Vorteile von Umgebungen
Es gibt verschiedene Gründe dafür, neben der Standardumgebung weitere Umgebungen zu erstellen:

- **Trennen der App-Entwicklung nach Abteilungen**: In einem großen Unternehmen kann jede Abteilung in einer anderen Umgebung arbeiten. Auf diese Weise werden den Mitarbeitern in einer Abteilung nur die Apps und Unternehmensdaten angezeigt, die deren Anforderungen entsprechen.
- **Unterstützen von Application Lifecycle Management (ALM):** Mit separaten Umgebungen können Sie Apps, die sich in den Entwicklungsphasen befinden, von denen trennen, die bereits freigegeben wurden. Alternativ kann eine Testumgebung von Vorteil sein, damit Sie Feedback von Mitarbeitern erhalten können, bevor Sie die endgültige App bereitstellen. Für einige Unternehmen kann das Anzeigen von Apps, bevor diese vollständig entwickelt und veröffentlicht wurden, zu Sicherheitsproblemen führen.
- **Verwalten des Zugriffs auf Daten:** Jede Umgebung kann über eine eigene Quelle von Unternehmensdaten verfügen, die als Common Data Service-Datenbank für Apps bezeichnet wird. Andere Datenverbindungen sind spezifisch für eine Umgebung und können nicht umgebungsübergreifend freigegeben werden.

> [!NOTE]
> Beachten Sie, dass Umgebungen nur für App-Ersteller und PowerApps-Administratoren relevant sind. Wenn Sie eine App für Benutzer freigeben, können diese Benutzer die App einfach ausführen, vorausgesetzt, sie verfügen über die erforderlichen Berechtigungen. Sie müssen sich keine Gedanken darüber machen, aus welcher Umgebung die App stammt.

## <a name="create-an-environment"></a>Erstellen einer Umgebung

Nur Administratoren können Umgebungen erstellen. Wenn Sie kein Administrator sind, können diese Informationen trotzdem für Sie hilfreich sein, wenn Sie das Einrichten von Umgebungen mit Ihrem Administrator besprechen.

1. Klicken Sie auf der Homepage von „web.powerapps.com“ in der oberen rechten Ecke auf das Zahnradsymbol, und wählen Sie **Admin Center** aus.

    Sie können admin.powerapps.com auch direkt öffnen.

2. Klicken Sie im PowerApps Admin Center auf **Neue Umgebung**. 
3. Geben Sie im Dialogfeld **Neue Umgebung** einen Namen für die Umgebung ein, und wählen Sie eine Region und einen Umgebungstyp aus.
4. Klicken Sie auf **Umgebung erstellen**.

Das ist alles. Sie verfügen nun über eine neue Umgebung, in der Sie arbeiten können. Wenn Sie zurück zu web.powerapps.com navigieren, wird sie in der Liste mit den Umgebungen angezeigt.

## <a name="manage-access-to-an-environment"></a>Verwalten des Zugriffs auf eine Umgebung

Standardmäßig können Sie mit einer der folgenden Methoden auf eine Umgebung zugreifen:

- **Systemadministratoren**: Ein Systemadministrator verfügt über die vollständigen Berechtigungen zum Erstellen und Verwalten von Umgebungen.
- **Umgebungsersteller**: Ein Umgebungsersteller kann alle Apps in dieser Umgebung anzeigen, Apps erstellen und mit Common Data Service für Apps arbeiten (hierfür sind weitere Berechtigungen erforderlich).

Administratoren können bei Bedarf weitere Sicherheitsrollen erstellen und diesen Benutzer zuweisen, wie in diesem Verfahren beschrieben.

1. Klicken Sie auf der linken Seite auf **Umgebungen**.
2. Wählen Sie eine Umgebung aus, und klicken Sie dann auf **Sicherheit für diese Instanz verwalten**.
3. Geben oder fügen Sie im Suchfeld rechts oben die E-Mail-Adresse der Person ein, der Sie Zugriff gewähren möchten.
4. Zeigen Sie auf das gewünschte Ergebnis, aktivieren Sie das entsprechende Kontrollkästchen, und wählen Sie dann **Rollen verwalten** aus.
5. Wählen Sie im Feld **Benutzerrollen verwalten** die Rollentypen für den Benutzer aus. In diesem Beispiel wurde dem Benutzer die Rolle „Umgebungsersteller“ zugewiesen.

    ![Auswählen einer neuen Benutzerrolle](../media/powerapps-user-roles.png)

6. Klicken Sie auf **OK**.

In dieser Einheit wurde erläutert, welche Vorteile Umgebungen bieten, wie sie erstellt werden und wie der Zugriff auf sie gewährt wird. Auch wenn Sie kein Administrator sind, können diese Informationen hilfreich sein.