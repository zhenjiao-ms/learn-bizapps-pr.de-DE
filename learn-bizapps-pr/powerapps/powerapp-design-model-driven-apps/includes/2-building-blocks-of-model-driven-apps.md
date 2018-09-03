Eine modellgesteuerte App besteht aus mehreren Komponenten, die Sie mithilfe des App-Designers auswählen. Die Komponenten und Komponenteneigenschaften werden die Metadaten. Diese Komponenten betrachten wir genauer.

## <a name="data"></a>Daten
Die Datenkomponenten bestimmen, auf welchen Daten die App basieren wird.

| Komponente        | Beschreibung | Designer |
|------------------|-------------|----------|
| Entität           | Entitäten sind Elemente mit Eigenschaften, die Sie nachverfolgen. Kontakte und Konten sind Beispiele hierfür. Es stehen viele Standardentitäten zur Verfügung. Sie können eine nicht zum System gehörige Standardentität (oder Produktionsentität) anpassen. Sie können auch eine benutzerdefinierte Entität von Grund auf neu erstellen. | Entity Designer |
| Feld            | Felder sind Eigenschaften, die einer Entität zugeordnet sind und zu ihrer Definition beitragen. Ein Feld wird durch einen Datentyp definiert, der den Typ der Daten bestimmt, die eingegeben oder ausgewählt werden können. Beispiele für Datentypen sind Text, Zahl, Datum und Uhrzeit, Währung und Nachschlagen (Erstellen einer Beziehung mit einer anderen Entität). Felder werden in der Regel mit Formularen, Ansichten und Suchvorgängen verwendet. | Entity Designer |
| Beziehung     | Beziehungen definieren, wie Entitäten miteinander verknüpft werden können. Es gibt 1:N (eins-zu-viele), N:1 (viele-zu-eins) und N:N (viele-zu-viele) Beziehungen. So erstellt z.B. das Hinzufügen eines Nachschlagefelds zu einer Entität eine neue 1:N-Beziehung zwischen den beiden Entitäten und ermöglicht Ihnen, dieses Nachschlagefeld einem Formular hinzuzufügen. | Entity Designer |
| Optionssatzfeld | Diese Art von Feld zeigt ein Steuerelement an, das dem Benutzer ermöglicht, unter vordefinierten Optionen auszuwählen. Jede Option verfügt über einen Zahlenwert und eine Bezeichnung. Optionssatzfelder können entweder einen einzelnen Wert oder mehrere Werte erfordern. | Entität |

## <a name="user-interface"></a>Benutzeroberfläche
Die Komponenten der Benutzeroberfläche bestimmen, wie Benutzer mit der App interagieren. 

| Komponente | Beschreibung | Designer |
|-----------|-------------|----------|
| App       | Apps bestimmen die App-Grundlagen wie Komponenten, Eigenschaften, Clienttyp und URL. | App-Designer |
| Siteübersicht  | Eine Siteübersicht legt die Navigation für Ihre App fest. | Designer für die Siteübersicht |
| Form      | Formulare enthalten eine Reihe von Dateneingabefeldern für eine bestimmte Entität. Dieser Satz von Dateneingabefeldern entspricht den Elementen, die Ihre Organisation für die Entität nachverfolgt. Ein Beispiel ist eine Reihe von Dateneingabefeldern, in die Benutzer relevante Informationen zur Nachverfolgung von vorherigen Bestellungen eines Kunden zusammen mit Datumsangaben bestimmter angeforderter Nachbestellungen eingeben. | Formulardesigner |
| Sicht      | Ansichten definieren, wie eine Liste mit Datensätzen für eine bestimmte Entität in Ihrer App angezeigt wird. Eine Ansicht definiert die anzuzeigenden Spalten, die Breite jeder Spalte, das Sortierverhalten und die Standardfilter. | Ansicht-Designer |

![App-Designer und Formulardesigner](../media/app-and-form-designers.png)

## <a name="logic"></a>Logik
Die Logikkomponenten bestimmen, welche Geschäftsprozesse, Regeln und Automatisierung die App hat. Microsoft PowerApps-Entwickler verwenden einen spezifischen Designer für den Prozess- oder Regeltyp.

| Logiktyp         | Beschreibung | Designer |
|-----------------------|-------------|----------|
| Geschäftsprozessflow | Geschäftsprozessflows führen Benutzer durch einen Standardgeschäftsprozess. Verwenden Sie einen Geschäftsprozessflow, wenn alle Mitarbeiter Kundendienstanforderungen in gleicher Weise behandeln sollen. Sie können auch mittels eines Geschäftsprozessflows regeln, dass Mitarbeiter vor dem Absenden einer Bestellung die Genehmigung für eine Rechnung einholen müssen. | Geschäftsprozessflow-Designer |
| Workflow              | Workflows automatisieren Geschäftsprozesse ohne Benutzeroberfläche. Designer verwenden Workflows, um die Automatisierung zu initiieren, die keine Benutzerinteraktion erfordert. | Workflow-Designer |
| Aktionen               | Aktionen sind Prozesstypen, mit denen Sie Aktivitäten, einschließlich benutzerdefinierter Aktivitäten, direkt aus einem Workflow manuell aufrufen können. | Prozessdesigner |
| Geschäftsregel         | Mit Geschäftsregeln werden Regeln oder Empfehlungslogik auf ein Formular angewandt, um Feldanforderungen, Ausblenden von Feldern, Überprüfen von Daten und Sonstiges festzulegen. App-Designer verwenden eine einfache Schnittstelle zum Implementieren und Verwalten sich schnell ändernder und häufig verwendeter Regeln. | Geschäftsregeldesigner |
| Flow                  | Microsoft Flow ist ein cloudbasierter Dienst, mit dem Sie automatisierte Workflows zwischen Apps und Diensten erstellen können, um Benachrichtigungen zu erhalten, Dateien zu synchronisieren, Daten zu sammeln und Sonstiges auszuführen. | Microsoft Flow |

![Workflow-, Aktions- und Geschäftsprozessflow-Designer](../media/designer-mash.png)

## <a name="visualization"></a>Visualisierung
Die Visualisierungkomponenten bestimmen, welche Art von Daten und Berichterstattung die App anzeigt.

| Komponente                   | Beschreibung | Designer |
|-----------------------------|-------------|----------|
|Diagramm                        | Diagramme sind einzelne grafische Visualisierungen, die in einer Ansicht oder einem Formular angezeigt oder einem Dashboard hinzugefügt werden können. | Diagramm-Designer |
|Dashboard                    | Dashboards zeigen eine oder mehrere grafische Visualisierungen an, die eine Übersicht über handlungsrelevante Geschäftsdaten bieten. | Dashboard-Designer |
| Microsoft Power BI Embedded | Power BI fügt Ihrer App eingebettete Power BI-Kacheln und Dashboards hinzu. Power BI ist ein cloudbasierter Dienst, der Einblicke in Business Intelligence (BI) bereitstellt. | Eine Kombination aus Diagramm-Designer, Dashboard-Designer und Power BI |

![Beispieldashboard](../media/dashboard-designer.png)

## <a name="advanced-model-driven-app-making"></a>Erweiterte Erstellung modellgesteuerter Apps
Der Projektmappen-Explorer wird zum Erstellen erweiterter modellgesteuerter Apps verwendet. Im Navigationsbereich auf der linken Seite des Tools können Sie in einer aus allen App-Komponenten bestehenden Hierarchie navigieren.

![Projektmappen-Explorer](../media/solutionexplorer-entitiescollapsed.png)