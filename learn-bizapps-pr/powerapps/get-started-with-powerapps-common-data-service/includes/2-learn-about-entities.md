Mit Common Data Service (CDS) für Apps können Sie schnell und einfach ein Datenmodell für Ihre Anwendung erstellen, das auf den Entitäten und den Entitätsmetadaten basiert, die Sie in Ihre App einbeziehen. 

Entitäten beschreiben die Arten von Daten, die in der CDS for Apps-Datenbank gespeichert werden. Jede Entität entspricht einer Datenbanktabelle, und jedes Feld (Attribut) einer Entität stellt eine Spalte in dieser Tabelle dar. 

*Metadaten* sind Daten über Daten. In CDS für Apps sind Metadaten eine Sammlung von Entitäten. Entitätsmetadaten steuern die Art der Datensätze, die Sie erstellen können, und die Art der Aktionen, die auf diese Datensätze angewendet werden können. Wenn Sie mit Anpassungstools Entitäten, Felder und Entitätsbeziehungen erstellen oder bearbeiten, werden diese Metadaten bearbeitet.

Die Apps, die Ihre Kunden zur Interaktion mit den Daten in Ihrer Umgebung verwenden, hängen von den Entitätsmetadaten ab und werden bei der Anpassung der Metadaten angepasst. 

## <a name="when-to-use-standard-entities-and-when-to-create-new-entities"></a>Wann werden Standardentitäten verwendet und wann neue Entitäten erstellt?
CDS für Apps bietet mehrere Standardentitäten, die die wichtigsten Funktionen für Geschäftsanwendungen unterstützen. Jede Entität weist außerdem mehrere Metadatenfelder auf, die allgemeine Daten darstellen, die das System für diese Entität speichern muss. Wir empfehlen, sich mit dem Katalog der Standardentitäten vertraut zu machen und sie nach Möglichkeit zu verwenden, da jede Anwendung, die mit Standardentitäten geschrieben wird, in Ihrer Umgebung ohne zusätzlichen Aufwand wie erwartet funktioniert.

Bei kleineren Änderungen müssen Sie möglicherweise keine benutzerdefinierte Entität erstellen: 

- Um den Anzeigenamen eines Felds zu ändern, können Sie die Entität bearbeiten. Sie müssen keine neue Entität erstellen.
- Standardentitäten können zwar nicht gelöscht, aber ausgeblendet werden. Um eine Standardentität auszublenden, ändern Sie die Berechtigungen für die Sicherheitsrolle in Ihrer Organisation so, dass das Leserecht für diese Entität entfernt wird. Dadurch wird die Entität aus den meisten Teilen der Anwendung entfernt.

Wenn Standardentitäten für Ihre Geschäftsanforderungen nicht geeignet sind bzw. nicht entsprechend bearbeitet werden können, sollten Sie das Erstellen einer neuen Entität, eines neuen Felds oder einer neuen Entitätsbeziehung erwägen. Wenn eine Standardentität Ihre geschäftlichen Anforderungen nahezu erfüllt, können Sie als Grundlage für eine neue Entität nutzen.

## <a name="entity-relationships"></a>Entitätsbeziehungen
Entitätsbeziehungen definieren die verschiedenen Möglichkeiten, wie Entitätsdatensätze mit Datensätzen aus anderen Entitäten oder derselben Entität verknüpft werden können. Entitätsbeziehungen sind Metadaten. Sie ermöglichen Abfragen einen sehr effizienten Abruf zusammengehöriger Daten. Nutzen Sie Entitätsbeziehungen, um die formalen Beziehungen zu definieren, die die Entität definieren oder die die meisten Datensätze verwenden können. 

Es gibt zwei Arten von Entitätsbeziehungen:

- **1:n-Beziehungen**: In einer 1:n-Entitätsbeziehung sind viele zusammengehörige Entitätsdatensätze einem einzelnen primären Entitätsdatensatz in einer Über-/Unterordnungsbeziehung zugeordnet. 
- **m:n-Beziehungen**: In einer m:n-Entitätsbeziehung sind viele Entitätsdatensätze vielen anderen Entitätsdatensätzen zugeordnet. Datensätze, die über m:n-Entitätsbeziehungen verknüpft sind, werden als Peers bezeichnet.

Neben der Definition, wie Datensätze mit anderen Datensätzen in Beziehung gesetzt werden können, bieten 1:n-Entitätsbeziehungen auch Daten zur Beantwortung der folgenden Fragen:

- Wenn ich einen Datensatz lösche, sollten dann auch alle Datensätze, die sich auf diesen Datensatz beziehen, gelöscht werden?
- Wenn ich einen Datensatz einem neuen Besitzer zuweise, muss ich dann auch alle zugehörigen Datensätze dem neuen Besitzer zuweisen?
- Wie kann ich den Dateneingabeprozess optimieren, wenn ich einen neuen Beziehungsdatensatz im Kontext eines bestehenden Datensatzes erstelle?
- Wie sollten Personen, die einen Datensatz anzeigen, die zugehörigen Datensätze einsehen können?

## <a name="entity-types"></a>Entitätstypen
Vor dem Erstellen oder Bearbeiten von Entitäten in CDS für Apps ist es ratsam, die verschiedenen Arten von Entitäten kennenzulernen, die Sie erstellen können. Nach der Erstellung einer benutzerdefinierten Entität können Sie den Entitätstyp nicht ändern. 

### <a name="types-of-entity-owners"></a>Typen von Entitätsbesitzern
Wenn Sie eine benutzerdefinierte Entität erstellen, sind die Optionen für den Besitz *Im Besitz von Benutzern/Team* und *Im Besitz der Organisation*. Nach der Erstellung einer Entität können Sie den Besitz nicht ändern. 

- **Im Besitz von Benutzern/Team**: Aktionen, die auf diese Datensätze angewendet werden können, lassen sich auf Benutzerebene steuern.
- **Im Besitz der Organisation**: Der Zugriff auf die Daten wird auf Organisationsebene gesteuert.

### <a name="activity-entities"></a>Aktivitätsentitäten
Eine *Aktivität* ist eine Aktion, für die ein Kalendereintrag erstellt werden kann. Aktivitäten haben folgende Merkmale:

- Zeitdimensionen (Startzeit, Endzeit, Fälligkeitsdatum und Dauer), die helfen zu definieren, wann die Aktion stattgefunden hat oder stattfinden wird.
- Daten (wie ein Thema und eine Beschreibung), die helfen, die Aktion zu definieren, die die Aktivität darstellt. 
- Lassen sich öffnen, abbrechen oder abschließen. Mehrere Teilstatuswerte werden dem Status *Abgeschlossen* einer Aktivität zugeordnet, um zu klären, wie die Aktivität abgeschlossen wurde. 
 
Aktivitätsentitäten können nur im Besitz eines Benutzers oder Teams sein. Sie können nicht einer Organisation gehören.

Die folgenden Standardaktivitätsentitäten sind verfügbar:

- **Termin**: Eine Verpflichtung, die ein Zeitintervall darstellt, das eine Anfangs-/Endzeit und Dauer aufweist.
- **E-Mail**: Eine Aktivität, die mithilfe von E-Mail-Protokollen zugestellt wird.
- **Fax**: Eine Aktivität, die für ein Fax das Anrufergebnis und die Anzahl der Seiten nachverfolgt. Die Aktivität kann optional eine elektronische Kopie des Dokuments speichern.
- **Brief**: Eine Aktivität, die die Zustellung eines Briefs nachverfolgt. Die Aktivität kann eine elektronische Kopie des Briefs speichern.
- **Telefonanruf**: Eine Aktivität, die einen Telefonanruf nachverfolgt.
- **Terminserie**: Der Mastertermin einer Terminserie.
- **Aufgabe**: Eine allgemeine Aktivität, die den erforderlichen Aufwand darstellt.

### <a name="custom-activity-entities"></a>Benutzerdefinierte Aktivitätsentitäten
Sie können neue benutzerdefinierte Aktivitätsentitäten erstellen. Die Metadatenwerte von Aktivitätsentitäten unterscheiden sich von den Metadatenwerten anderer Entitäten. Das Feld **Primär** ist beispielsweise auf **Betreff** festgelegt. 

Sie können im Microsoft PowerApps-Portal keine benutzerdefinierte Aktivität erstellen. Sie müssen den Projektmappen-Explorer über die Schaltfläche **Erweitert** öffnen. 
