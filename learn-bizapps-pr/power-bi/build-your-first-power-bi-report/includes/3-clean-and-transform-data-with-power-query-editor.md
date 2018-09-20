Nachdem wir uns über **Microsoft Power BI Desktop** mit einer Datenquelle verbunden haben, müssen wir die Daten an unsere Bedürfnisse anpassen. Anpassen von Daten bedeutet mitunter das *Transformieren* der Daten, wie z.B. Umbenennen von Spalten oder Tabellen, Ändern von Text in Zahlen, Entfernen von Zeilen oder Festlegen der ersten Zeile als Überschrift.

Der **Power Query-Editor** in Power BI Desktop ermöglicht nicht nur das Ausführen von Aufgaben über das Menüband, sondern auch über zahlreiche Kontextmenüs, die durch Klicken mit der rechten Maustaste geöffnet werden. Die meisten Optionen, die Sie auf dem Menüband auf der Registerkarte **Transformieren** auswählen können, sind auch verfügbar, wenn Sie mit der rechten Maustaste auf ein Element (z.B. eine Spalte) klicken und im angezeigten Kontextmenü einen Befehl auswählen.

## <a name="shape-data"></a>Strukturieren von Daten
Wenn Sie Daten im **Power Query-Editor** *strukturieren*, geben Sie eine Schritt-für-Schritt-Anleitung vor, die der **Power Query-Editor** für Sie befolgt, um das Laden und Präsentieren der Daten anzupassen. Die ursprüngliche Datenquelle ist nicht betroffen. Nur diese bestimmte Ansicht der Daten wird angepasst bzw. *strukturiert*.

Die von Ihnen angegebenen Schritte (z. B. Tabelle umbenennen, Datentyp transformieren oder Spalten löschen) werden von **Power Query Editor** aufgezeichnet. Diese Schritte werden dann bei jeder Verbindung der Abfrage mit der Datenquelle ausgeführt, sodass die Daten immer so strukturiert werden, wie Sie es wünschen. Dieser Prozess erfolgt immer dann, wenn Sie die Abfrage in Power BI Desktop verwenden oder jemand anderes Ihre freigegebene Abfrage verwendet (z.B. im **Power BI-Dienst**). Die Schritte werden im Bereich **Power Query-Einstellungen** unter **Angewendete Schritte** sequenziell erfasst.

Die folgende Abbildung zeigt den Bereich **Abfrageeinstellungen** für eine Abfrage, die bereits strukturiert ist. In den nächsten Abschnitten werden wir jeden dieser Schritte durchgehen.

![Fertige Abfrageeinstellungen](../media/pbid-clean-xform_01.png)

Kehren wir zurück zu den Daten für Pensionäre, die wir über die Verbindung mit einer Datenquelle im **Web** gefunden haben. Lassen Sie uns die Daten so strukturieren, dass sie unseren Anforderungen entsprechen.

Zunächst einmal wurden die meisten Bewertungen in **Power Query-Editor** als ganze Zahlen eingegeben, aber einige nicht. Da eine Spalte Text und Zahlen enthielt, wurde sie nicht automatisch konvertiert. Power BI erkennt diese Änderungen häufig und ändert automatisch den Datentyp. 

Wir benötigen die Daten als Zahlen. Kein Problem: Klicken Sie einfach mit der rechten Maustaste auf die Spaltenüberschrift, und wählen Sie zum Ändern des Datentyps **Typ ändern \> Ganze Zahl** aus. Wenn Sie mehr als eine Spalte ändern müssen, wählen Sie eine davon aus, und halten Sie dann die **UMSCHALTTASTE** gedrückt, während Sie weitere benachbarte Spalten auswählen. Klicken Sie dann mit der rechten Maustaste auf eine Spaltenüberschrift, um alle ausgewählten Spalten zu ändern. Bei gedrückter **STRG-Taste** können wir auch nicht benachbarte Spalten auswählen.

![Fertige Abfrageeinstellungen](../media/pbid-clean-xform_02.png)

> [!NOTE]
> Häufig erkennt Power Query, dass eine Textspalte Zahlen enthalten sollte, und ändert automatisch den Datentyp, wenn die Tabelle in den Power Query Editor übertragen wird. In diesem Fall gibt ein Schritt unter **Anwendete Schritte** Auskunft darüber, was Power Query für Sie getan hat.

Sie können den Typ dieser Spalten auch auf dem Menüband auf der Registerkarte **Transformieren** von Text in Überschrift ändern bzw. *transformieren*. Die folgende Abbildung zeigt die Registerkarte **Transformieren**. Der Pfeil zeigt auf die Schaltfläche **Datentyp**, die Ihnen ermöglicht, den aktuellen Datentyp in einen anderen zu transformieren.

![Die Registerkarte „Transformieren“ und die Schaltfläche „Datentyp“](../media/pbid-clean-xform_02b.png)

Beachten Sie, dass im Bereich **Abfrageeinstellungen** die vorgenommenen Änderungen unter **Angewendete Schritte** übernommen wurden. Um einen Schritt aus dem Strukturierungsprozess zu entfernen, wählen Sie ihn einfach aus, und klicken Sie dann links daneben auf das **X**.

![Fenster „Abfrageeinstellungen“](../media/pbid-clean-xform_03.png)

## <a name="connect-to-data"></a>Herstellen einer Verbindung mit Daten
Diese Daten über verschiedene US-Bundesstaaten sind interessant und für zusätzliche Analyseaktivitäten und Abfragen nützlich. Doch es gibt ein Problem: Bei den meisten Daten wird ein Kürzel aus zwei Buchstaben für US-Bundesstaatcodes verwendet, nicht der vollständige Name des US-Bundesstaats. Wir benötigen deshalb eine Möglichkeit, Bundesstaatsnamen mit ihren Kürzeln zu verknüpfen.

Wir haben Glück: Es gibt eine andere öffentliche Datenquelle, die genau diese Aufgabe erfüllt. Aber es bedarf einer gewissen Strukturierung, bevor wir sie mit unserer Tabelle für Pensionäre verbinden können. Hier finden Sie die Webressource mit den US-Bundesstaatskürzeln:

<http://en.wikipedia.org/wiki/List_of_U.S._state_abbreviations>

Klicken Sie im **Power Query-Editor** auf der Registerkarte **Start** auf das Menüband und dann auf **Neue Quelle \> Web**. Geben Sie dann die Adresse ein, und klicken Sie auf **OK**. Das Fenster **Navigator** zeigt, was auf dieser Webseite gefunden wurde.

![Von Website abgerufene Kürzel der US-Bundesstaaten](../media/pbid-clean-xform_04.png)

Wählen Sie **Codes and abbreviations...** aus, da diese Tabelle die gewünschten Daten enthält. Sie muss aber noch so strukturiert werden, dass sie nur noch die gewünschten Daten enthält. 

Klicken Sie auf **OK**, um die Daten in den **Power Query-Editor** zu übertragen, damit wir sie strukturieren können. Führen Sie dann die folgenden Schritte durch:

* **Entfernen Sie die ersten drei Zeilen**: Diese Zeilen haben sich aufgrund der Erstellung der Tabelle auf der Webseite ergeben und werden von uns nicht benötigt. Um sie zu entfernen, wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Spalten entfernen \> Erste Zeilen entfernen** aus. Geben Sie im angezeigten Dialogfeld *3* als Anzahl der Zeilen ein, die entfernt werden soll.

    ![Erste Zeilen entfernen](../media/pbid-clean-xform_04a.png)

* **Entfernen Sie die letzten 26 Zeilen**: Diese Zeilen gehören alle zu Gebieten, die wir nicht einbeziehen möchten. Der Prozess ist identisch, aber dieses Mal wählen Sie **Zeilen entfernen \> Untere Zeilen entfernen** aus und geben dann *26* als Anzahl der Zeilen ein, die entfernt werden sollen.

    ![Untere Zeilen entfernen](../media/pbid-clean-xform_04b.png)

* **Filtern Sie Washington, D.C. heraus**: Die Tabelle mit den Statistiken für Pensionäre enthält Washington, D.C. nicht, weshalb wir diesen Eintrag aus unserer Liste entfernen können. Klicken Sie auf den Dropdownpfeil neben der Spalte **Name and status of region2**, und deaktivieren Sie dann das Kontrollkästchen neben **Federal district**. 

    ![Entfernen einer Zeile, die einen bestimmten Wert enthält](../media/pbid-clean-xform_04c.png)

* **Entfernen Sie mehrere überflüssige Spalten**: Wir brauchen nur die Zuordnung jedes Bundesstaats zu seinem offiziellen Kürzel aus zwei Buchstaben. Diese Informationen finden wir in der zweiten und fünften Spalte. Aus diesem Grund müssen wir nur diese beiden Spalten beibehalten und können alle anderen entfernen. Wählen Sie die erste zu entfernende Spalte aus, und klicken Sie dann bei gedrückter STRG-TASTE auf die anderen zu entfernenden Spalten (so können Sie mehrere nicht zusammenhängende Spalten auswählen). Wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Spalten entfernen \> Spalten entfernen** aus.

    ![Entfernen bestimmter Spalten](../media/pbid-clean-xform_04d.png)

* **Verwenden Sie die erste Zeile als Überschrift**: Da wir die ersten drei Zeilen entfernt haben, wird die aktuelle oberste Zeile zur gewünschten Überschrift. Klicken Sie auf die Schaltfläche **Erste Zeile als Überschriften verwenden**.

    ![Erste Zeile als Überschriften verwenden](../media/pbid-clean-xform_04e.png)

    > [!NOTE]
    > An dieser Stelle sei darauf hingewiesen, dass die *Reihenfolge* der im **Power Query-Editor** angewendeten Schritte wichtig ist und sich auf die Strukturierung der Daten auswirken kann. Es ist auch wichtig zu berücksichtigen, wie sich ein Schritt auf einen anderen nachfolgenden Schritt auswirken kann. Wenn Sie aus der Liste **Angewendete Schritte** einen Schritt entfernen, verhalten sich nachfolgende Schritte wegen des Einflusses der Schrittreihenfolge der Abfrage ggf. nicht mehr so wie ursprünglich beabsichtigt.

* **Benennen Sie die Spalten und die Tabelle selbst um**. Wie üblich gibt es mehrere Möglichkeiten, eine Spalte umzubenennen. Wählen Sie die von Ihnen bevorzugte Methode. Lassen Sie uns die Spalten in *State Name* und *State Code* umbenennen. Um die Tabelle umzubenennen, geben Sie einfach im Bereich **Abfrageeinstellungen** den Namen in das Feld **Name** ein. Wir nennen diese Tabelle *StateCodes*.

    ![Umbenennen von Spalten](../media/pbid-clean-xform_04f.png)

## <a name="combine-data"></a>Kombinieren von Daten

Nachdem die Tabelle **StateCodes** strukturiert wurde, können wir die beiden Tabellen zu einer kombinieren. Da die Tabellen, die wir jetzt haben, das Ergebnis der Abfragen sind, die wir auf die Daten angewendet haben, werden sie oft als *Abfragen* bezeichnet.

Zum Kombinieren von Abfragen gibt zwei Möglichkeiten: *Zusammenführen* und *Anfügen*.

Wenn eine oder mehrere Spalten zu einer anderen Abfrage hinzugefügt werden sollen, werden die Abfragen **zusammengeführt**. Wenn einer vorhandenen Abfrage zusätzliche Datenzeilen hinzugefügt werden sollen, wird die Abfrage **angefügt**.

In diesem Fall möchten wir die Abfragen zusammenführen. Wählen Sie zunächst die Abfrage, *mit* der die andere Abfrage zusammengeführt werden soll. Wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Abfragen zusammenführen**. Wir wählen zuerst unsere Abfrage von Daten für Pensionäre aus. Wenn wir schon mal dabei sind, benennen wir diese Abfrage in *RetirementStats* um.

![Schaltfläche „Abfragen zusammenführen“](../media/pbid-clean-xform_05.png)

Im eingeblendeten Dialogfeld **Zusammenführen** werden wir aufgefordert, die Tabelle auszuwählen, die mit der ausgewählten Tabelle zusammengeführt werden soll. Anschließend müssen wir die Spalten angeben, die für die Zusammenführung verwendet werden sollen. 

Wählen Sie **State** in der Tabelle (Abfrage) **RetirementStats** und dann die Abfrage **StateCodes** aus. (In diesem Fall ist die Wahl einfach, da nur eine andere Abfrage vorhanden ist. Wenn Sie eine Verbindung mit vielen Datenquellen herstellen, stehen jedoch viele Abfragen zur Auswahl.) Nachdem Sie die richtigen übereinstimmenden Spalten (**State** aus **RetirementStats** und **State Name** aus **StateCodes**) ausgewählt haben, sieht das Fenster **Zusammenführen** wie folgt aus, und die Schaltfläche **OK** ist verfügbar.

![Dialogfeld „Zusammenführen“](../media/pbid-clean-xform_06.png)

Am Ende der Abfrage wird eine neue Spalte namens **NewColumn** erstellt, die den Inhalt der Tabelle (Abfrage) enthält, die mit der vorhandenen Abfrage zusammengeführt wurde. Alle Spalten aus der zusammengeführten Abfrage werden auf die neue Spalte **NewColumn** zusammengefasst. Sie können jedoch die Tabelle **erweitern** und gewünschte Spalten einbeziehen. Um die zusammengeführte Tabelle zu erweitern und auszuwählen, welche Spalten einbezogen werden sollen, klicken Sie auf das Symbol „Erweitern“ (![Symbol „Erweitern“](../media/pbid-clean-xform_07.png)). Das Dialogfeld **Erweitern** wird angezeigt.

![Dialogfeld „Erweitern“](../media/pbid-clean-xform_08.png)

In diesem Fall beschränken wir uns auf die Spalte **State Code**. Wählen Sie deshalb nur diese Spalte aus, und klicken Sie dann auf **OK**. Sie können auch das Kontrollkästchen **Ursprünglichen Spaltennamen als Präfix verwenden** deaktivieren. Wenn das Kontrollkästchen aktiviert bleibt, erhält die zusammengeführte Spalte den Namen *NewColumn.State Code* (zusammengesetzt aus dem ursprünglichen Spaltennamen bzw. *NewColumn*, einem Punkt und dem Namen der in die Abfrage eingefügten Spalte).

> [!NOTE]
> Auf Wunsch können Sie damit experimentieren, wie die Tabelle **NewColumn** zum Einsatz kommt. Wenn Ihnen die Ergebnisse nicht gefallen, löschen Sie einfach im Bereich **Abfrageeinstellungen** in der Liste **Angewendete Schritte** den Schritt **Erweitern**. Ihre Abfrage kehrt zum Zustand zurück, in dem sie sich vor der Anwendung dieses Schritts befand. Auf diese Weise können Sie beliebig oft und solange experimentieren, bis die Erweiterung Ihren Vorstellungen entspricht.

Wir haben jetzt eine einzelne Abfrage (Tabelle), in der zwei entsprechend den Anforderungen strukturierte Datenquellen miteinander kombiniert sind. Diese Abfrage kann als Grundlage vieler weiterer interessanter Datenverbindungen dienen, z.B. für Statistiken zu Wohnkosten, demografischen Daten oder Beschäftigungsmöglichkeiten in den US-Bundesstaaten.

Um die Änderungen im **Power Query-Editor** zu übernehmen und sie in Power BI Desktop zu laden, wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Schließen und übernehmen**.

![Schließen und Übernehmen von Dateneinstellungen](../media/pbid-clean-xform_09.png)

Nun können Sie mit den Daten in Ihrem Modell arbeiten. Als Nächstes erstellen wir einige Visuals für Ihren Bericht.

Im Moment haben wir genügend Daten, um in Power BI Desktop eine Reihe interessanter Berichte zu erstellen. Da es sich um einen Meilenstein handelt, lassen Sie uns diese Power BI Desktop-Datei speichern. Wählen Sie auf der Registerkarte **Start** den Befehl **Datei \> Speichern**. Wir nennen den Bericht **Erste Schritte mit Power BI Desktop**.

Prima! Nun weiter zur nächsten Einheit, in der wir einige interessante Visuals erstellen.
