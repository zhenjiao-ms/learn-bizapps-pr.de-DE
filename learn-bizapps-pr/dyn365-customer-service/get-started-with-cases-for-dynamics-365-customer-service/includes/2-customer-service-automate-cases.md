In vielen Organisationen ist die Kundenservicefunktion in hohem Maße strukturiert. Der Kundenservice kann Zusagen zu Berechtigungen zur Vereinbarung zum Servicelevel (SLA), Anforderungen zum Nachverfolgen von Informationen, wie etwa der Dauer zur Lösung von Anfragen, und vieles mehr umfassen.

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE2ywCJ]

Aufgrund dieser Merkmale interagieren Aktivitätsdatensätze mit Anfragedatensätzen etwas anders als mit anderen Datensatztypen. Zwei der wichtigsten Unterschiede:

- Ein Anfragedatensatz kann nicht abgeschlossen werden, wenn er nicht abgeschlossene Aktivitäten enthält. Der Benutzer wird darüber informiert, dass offene Aktivitäten automatisch abgebrochen werden, wenn die Anfrage abgeschlossen wird.
- Wenn ein Anfragedatensatz abgeschlossen wird, wird die Dauer des Anfrageabschlussprozesses automatisch berechnet, indem die tatsächliche Zeit hinzugefügt wird, die für alle Aktivitäten aufgewandt wurde, die der Anfrage zugeordnet sind.

Beachten Sie, dass der Wert die benötigte Zeit möglicherweise nicht genau widerspiegelt, obwohl Microsoft Dynamics 365 for Customer Service die aufgewandte Gesamtzeit für eine Anfrage automatisch berechnet. Während des Abschlussprozesses kann der Benutzer die tatsächlich aufgewandte Gesamtzeit eingeben.

Der Zweck einer Anfrage ist es, Kundenprobleme, Fragen und Anforderungen nachzuverfolgen und diese über einen Abschluss zu verwalten. Gelegentlich senden Kunden eine Anforderung, ändern aber später ihre Meinung und beschließen, dass sie keine Hilfe mehr benötigen. Customer Service-Benutzer haben standardmäßig zwei Möglichkeiten, diese Situation zu bewältigen: Sie können die Anfrage stornieren oder löschen. 

## <a name="resolving-cases"></a>Abschließen von Anfragen 
Anfragen können auf unterschiedliche Weise abgeschlossen werden. Manchmal kann das Problem gelöst werden, ohne dass Recherchen oder die Nutzung anderer Ressourcen erforderlich sind. Ein anderes Mal muss der Kundenservicemitarbeiter das Problem untersuchen und die Wissensdatenbank durchsuchen, um zu sehen, wie andere Mitarbeiter ähnliche Probleme gelöst haben. Manchmal muss das Problem möglicherweise eskaliert werden. 

Eine Anfrage kann erst abgeschlossen werden, wenn sämtliche Aktivitäten, die mit ihr in Verbindung stehen, wie etwa Telefonanrufe, Briefe, Termine oder E-Mails, ebenfalls abgeschlossen sind. Dadurch wird verhindert, dass ein beliebiger Benutzer versehentlich eine Anfrage abschließt, bevor alle Workflows oder festgelegten Aktivitäten beendet sind.

### <a name="deleting-and-canceling-cases"></a>Löschen und Stornieren von Anfragen

Manchmal beschließen Kunden, dass sie keine Hilfe mehr benötigen. In diesem Fall haben Mitarbeiter zwei Optionen: sie können die Anfrage stornieren oder löschen. 

- **Löschen einer Anfrage**: Durch Löschen einer Anfrage werden alle Aktivitäten, Notizen und Anhänge entfernt, die der Anfrage zugeordnet sind. Beachten Sie, dass dies eine dauerhafte Aktion ist. Der Datensatz des Kundenproblems geht verloren.
- **Stornieren einer Anfrage**: Wenn Sie nicht sicher sind, ob der Datensatz in der Zukunft benötigt wird, stellt das Stornieren der Anfrage die bessere Wahl dar. Beim Stornieren einer Anfrage wird der Datensatz im System behalten, sodass er zu einem späteren Zeitpunkt wieder aktiviert werden kann, wenn er erneut benötigt wird. Beachten Sie, dass viele Organisationen die Sicherheitsrollen im Customer Service so konfigurieren, dass Benutzer keine Anfragen löschen können. Das hilft, falsche Löschvorgänge zu verhindern.

### <a name="reactivating-cases"></a>Erneutes Aktivieren von Anfragen

Wenn eine Anfrage geschlossen wurde, kann sie erneut aktiviert werden. Beispiel: Wenn ein Kunde bei einem Problem erneut anruft, kann der Kundenservicemitarbeiter die ursprüngliche Anfrage wieder aktivieren, statt eine neue Anfrage zu öffnen.

### <a name="assigning-case-records"></a>Zuweisen von Anfragedatensätzen
Nach dem Erstellen einer Anfrage kann jeder Kundenservicemitarbeiter sie einem anderen Mitarbeiter, einem anderen Benutzer im System oder einer Warteschlange zuweisen. 

Im Customer Service weisen zahlreiche Datensatztypen einen Besitzer auf. Der Besitz eines Datensatzes bedeutet, dass die Person oder das Team, die/das dem Datensatz als Besitzer zugeordnet ist, für die Verwaltung dieses Datensatzes zuständig ist. Wenn ein Geschäftsszenario eine Änderung des Besitzes für einen Datensatz erfordert, wird der Datensatz einer anderen Person oder einem anderen Teams zugewiesen.

### <a name="assigning-a-case-record-to-a-queue"></a>Zuweisen eines Anfragedatensatzes zu einer Warteschlange
Customer Service-Warteschlangen können verwendet werden, um bei Serviceverwaltungsszenarien zu helfen. Beispiel: Eine Warteschlange kann so konfiguriert werden, dass sie eingehende E-Mails entgegennimmt, die anschließend in Anfragen konvertiert werden.
