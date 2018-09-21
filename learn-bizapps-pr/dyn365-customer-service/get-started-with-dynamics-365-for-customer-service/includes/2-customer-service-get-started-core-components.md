Werfen wir nun einen Blick auf die grundlegenden Datensatztypen, die für die Serviceverwaltung verwendet werden.

## <a name="types-of-records"></a>Datensatztypen

**Kundendatensätze**: In Microsoft Dynamics 365 for Customer Service werden Kundenserviceanfragen in der Regel in Verbindung mit einem vorhandenen Kontakt- oder Firmendatensatz verwaltet. Diese Kontakte und Firmen werden auch von anderen Geschäftsbereichen verwendet, wie etwa Vertrieb oder Marketing. 

- Ein *Kontakt* stellt eine Person wie in Microsoft Outlook dar. 
- Eine *Firma* steht für ein Unternehmen, eine Organisation oder eine Gruppe von Personen. 

Auch wenn dies die üblichen Verwendungsarten von Firmen und Kontakten sind, verwenden unterschiedliche Customer Service-Bereitstellungen diese Datensatztypen möglicherweise unterschiedlich. Beide werden jedoch in der Regel als *Kunden* bezeichnet. Beispiel: Wenn Sie den Kunden in einer Anfrage eintragen, können Sie wählen, ob es sich um eine Firma oder einen Kontakt handelt.

**Anfragen**: Bei einer Anfrage handelt es sich um den grundsätzlichen Datensatztyp in der Serviceverwaltung. Sie steht für einen einzelnen Fall eines angeforderten Service. Verschiedene Organisationen verwenden möglicherweise verschiedene Begriffe für die Bezeichnung von Anfragen: *Vorfall*, *Ticket*, *Serviceanfrage* usw. 

In anderen Worten stehen Anfragen für alles im Kontext einer Kundeninteraktion, die den Typ „Lösung“ oder „Antwort“ erfordert. Einem einzelnen Kundendatensatz können jederzeit viele Anfragen zugeordnet sein. Im Customer Service können Mitarbeiter die offenen und abgeschlossenen Anfragen aus dem Kundendatensatz anzeigen.

**Aktivitäten**: Interaktionen zwischen einem Unternehmen und seinen Kunden, die als wichtig genug für die Nachverfolgung betrachtet werden, werden im Customer Service als *Aktivitäten* bezeichnet. Aktivitäten können zahlreichen Arten von Datensätzen im Customer Service zugeordnet werden. Sie können den Datensatz öffnen und die Aktivitäten unter **Abgeschlossene Aktivitäten** oder **Offene Aktivitäten** suchen. 

- Abgeschlossene Aktivitäten wurden als abgeschlossen markiert.
- Öffnen Aktivitäten wurden entweder nicht als abgeschlossen markiert oder ihr Abschluss steht an einem anderen Datum und zu einer anderen Uhrzeit noch aus.

**Berechtigungen**: Berechtigungen können verwendet werden, um anzugeben, zu wie vielen Supportservices ein Kunde berechtigt ist. Beispiel: Die Berechtigung eines Kunden im Customer Service lässt zehn Supportanfragen zu, die der Kunde im eigenen Ermessen verwenden kann. 

**Berechtigungskanäle**: Berechtigungskanäle können verwendet werden, um die Art des Service anzugeben, zu dem ein Kunde berechtigt ist. Es gibt fünf Berechtigungskanäle:

- Telefon
- E-Mail
- Web
- Facebook
- Twitter

**Wissensdatenbankartikel**: Die Wissensdatenbankartikel im Customer Service sind ein Repository an Informationsartikeln, die Kundenservicemitarbeitern beim Abschließen von Anfragen helfen. In einigen Organisationen helfen die Informationen in der Wissensdatenbank den Mitarbeitern nicht nur beim Beheben von Problemen, sondern stellen auch Nachverfolgungsfragen.

Normalerweise handelt es sich bei diesen Informationen um Informationen zum Unternehmen, Produktfragen und -antworten und jegliche andere Art von Informationen, die Mitarbeitern helfen können, Kundenanfragen, -anforderungen oder -probleme besser abzuwickeln.

**Abschlussaktivitäten**: Nach dem Abschluss aller Aktivitäten für eine Anfrage kann die Anfrage selbst abgeschlossen werden. Nach dem Abschluss der Anfrage wird eine Aktivität vom Typ **Abschlussaktivität** erstellt. Diese Aktivität befindet sich unter den abgeschlossenen Aktivitäten, die einer Anfrage zugeordnet sind. Abschlussaktivitäten zeigen den Abschluss der Anfrage und die für die Anfrage aufgewandte Zeit.

**Warteschlangen**: Eine Warteschlange ist ein Ort zum Organisieren und Speichern von Aktivitäten und Anfragen, die auf die Verarbeitung warten.

Beispiel: Eine Organisation kann über ein Supportteam mit der E-Mail-Adresse `support@contoso.com` verfügen. Wenn das Supportteam unter dieser Adresse eine E-Mail erhält, behandelt ein Mitglied des Teams die Supportanfrage und arbeitet an der Lösung des Problems für den Kunden. 

Warteschlangen in Microsoft Dynamics funktionieren identisch.

**Produkte**: Produkte im Microsoft Dynamics CRM-Produktkatalog können einer Kundenserviceanfrage zugeordnet werden. Daher können sie helfen, eine detailliertere Ansicht der Anfragen, Abschlüsse und Kundenfeedbacks auf Produktebene bereitzustellen.

Auch wenn Produkte Anfragen zugeordnet werden können, um die Typen der Anfragen besser zu kategorisieren, hat diese Zuordnung keine Auswirkungen auf die Preise oder die Rechnung. Darüber hinaus ist die Verwendung von Produkten zusammen mit Anfragen optional und möglicherweise nicht auf alle Organisationen anwendbar.

**Ziele**: Neben der Berichterstellung und Analyse der Informationen im Customer Service können Organisationen die Zielverwaltungsfunktionen verwenden, um Zielwerte für die Key Performance Indicators (KPIs) einzurichten und den Fortschritt nachzuverfolgen. Im Servicemanagement können diese KPIs Kennzahlen enthalten, wie etwa abgeschlossene Anfragen oder Anfragen in Bearbeitung.

**Vereinbarungen zum Servicelevel**: Vereinbarungen zum Servicelevel (SLA) stellen eine Möglichkeit der Nachverfolgung und Definition dar, was geschehen soll, wenn eine Anfrage geöffnet wird. Sie können Aspekte nachverfolgen, wie etwa, wann eine Anfrage erstmals von einem Supporttechniker aufgenommen wurde und wie lange es dauerte, die Anfrage abzuschließen. Sie können auch E-Mails auf Grundlage bestimmter Warnungs- und Fehlerzeitachsen senden.