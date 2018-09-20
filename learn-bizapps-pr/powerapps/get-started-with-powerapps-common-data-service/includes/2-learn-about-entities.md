Mit Common Data Service (CDS) für Apps können Sie schnell und einfach ein Datenmodell für Ihre Anwendung erstellen, das auf den Entitäten und den Entitätsmetadaten basiert, die Sie in Ihre App einbeziehen. 

Mit Entitäten wird beschrieben, welche Arten von Daten in der Datenbank für Common Data Service für Apps gespeichert werden. Jede Entität entspricht einer Datenbanktabelle, und jedes Feld (auch als Attribut bezeichnet) innerhalb einer Entität stellt eine Spalte in dieser Tabelle dar. 

In Common Data Service für Apps sind Metadaten (also Daten über Daten) eine Sammlung von Entitäten. Mit Entitätsmetadaten wird angegeben, welche Datensätze Sie erstellen können und welche Aktionen sich für diese ausführen lassen. Wenn Sie mit Anpassungstools Entitäten, Felder und Entitätsbeziehungen erstellen oder bearbeiten, werden diese Metadaten bearbeitet.

Die Apps, die Ihre Kunden zur Interaktion mit den Daten in Ihrer Umgebung verwenden, sind von den Entitätsmetadaten abhängig und werden bei der Anpassung der Metadaten entsprechend geändert. 

<<<<<<< KOPFTEIL
## <a name="when-to-use-standard-entities-and-when-to-create-new-entities"></a>Wann sollten Standardentitäten und neue Entitäten erstellt werden?
<a name="common-data-service-for-apps-comes-with-a-number-of-standard-entities-that-support-core-business-application-capabilities-each-entity-also-contains-a-number-of-metadata-fields-that-represent-common-data-that-the-system-needs-to-store-for-that-entity-we-recommend-that-you-become-very-familiar-with-the-catalog-of-standard-entities-and-use-them-where-possible-because-any-applications-written-with-standard-entities-will-work-as-you-expect-in-your-environment-without-additional-effort"></a>Common Data Service für Apps bietet mehrere Standardentitäten, die die wichtigsten Funktionen für Geschäftsanwendungen unterstützen. Jede Entität enthält außerdem eine Reihe von Metadatenfeldern. Diese stellen allgemeine Daten dar, die das System für diese Entität speichern muss. Es wird empfohlen, dass Sie sich mit dem Katalog der Standardentitäten genau vertraut machen und diese nach Möglichkeit verwenden, da jede Anwendung, die mit Standardentitäten geschrieben wird, in Ihrer Umgebung ohne zusätzlichen Aufwand wie erwartet funktioniert.
=======
## <a name="when-to-use-standard-entities-and-when-to-create-new-entities"></a>Wann sollten Standardentitäten und neue Entitäten erstellt werden?
CDS für Apps bietet mehrere Standardentitäten, die die wichtigsten Funktionen für Geschäftsanwendungen unterstützen. Jede Entität weist außerdem mehrere Metadatenfelder auf, die allgemeine Daten darstellen, die das System für diese Entität speichern muss. Es wird empfohlen, dass Sie sich mit dem Katalog der Standardentitäten vertraut machen und diese nach Möglichkeit verwenden, da jede Anwendung, die mit Standardentitäten geschrieben wird, in Ihrer Umgebung ohne zusätzlichen Aufwand wie erwartet funktioniert.
>>>>>>> master

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
<<<<<<< KOPFTEIL Vor dem Erstellen oder Bearbeiten von Entitäten in Common Data Service für Apps sollten Sie die verschiedenen Entitätstypen verstehen, die Sie erstellen können. Nach der Erstellung einer benutzerdefinierten Entität kann der Entitätstyp nicht mehr geändert werden. 

### <a name="types-of-entity-owners"></a>Typen von Entitätsbesitzern
 <a name="when-you-create-a-custom-entity-the-options-for-ownership-are-user-or-team-owned-or-organization-owned-after-an-entity-is-created-you-cant-change-the-ownership"></a>Wenn Sie eine benutzerdefinierte Entität erstellen, stehen als Besitzoptionen *User or team owned* (Im Besitz der Benutzer/des Teams) und *Organization-owned* (Im Besitz der Organisation) zur Auswahl. Nach der Erstellung einer Entität können Sie den Besitz nicht ändern. 
=======
Vor dem Erstellen oder Bearbeiten von Entitäten in CDS für Apps ist es ratsam, die verschiedenen Entitätstypen kennenzulernen, die Sie erstellen können. Nach der Erstellung einer benutzerdefinierten Entität können Sie den Entitätstyp nicht ändern. 

### <a name="types-of-entity-owners"></a>Typen von Entitätsbesitzern
Wenn Sie eine benutzerdefinierte Entität erstellen, sind die Optionen für den Besitz *Im Besitz von Benutzern/Team* und *Im Besitz der Organisation*. Nach der Erstellung einer Entität können Sie den Besitz nicht ändern. 
>>>>>>> master

- **User or team owned** (Im Besitz der Benutzer/des Teams): Aktionen, die auf diese Datensätze angewendet werden können, lassen sich auf Benutzerebene steuern.
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
