Nachdem wir uns über **Power BI Desktop** mit einer Datenquelle verbunden haben, müssen wir die Daten an unsere Bedürfnisse anpassen. Das Anpassen von Daten bedeutet mitunter das *Transformieren* der Daten, wie z.B. Umbenennen von Spalten oder Tabellen, Ändern von Text in Zahlen, Entfernen von Zeilen, Festlegen der ersten Zeile als Überschrift usw.

Der **Power Query-Editor** in Power BI Desktop ermöglicht nicht nur das Ausführen von Aufgaben über das Menüband, sondern auch über zahlreiche Kontextmenüs. Die meisten Optionen, die Sie auf dem Menüband **Transformieren** auswählen können, sind auch verfügbar, indem Sie mit der rechten Maustaste auf ein Element (z.B. eine Spalte) klicken und im angezeigten Menü die gewünschte Option auswählen.

## <a name="shape-data"></a>Strukturieren von Daten
Wenn Sie Daten im **Power Query-Editor** strukturieren, geben Sie eine Schritt-für-Schritt-Anleitung vor (die der **Power Query-Editor** für Sie umsetzt), um die Daten so anzupassen, wie sie vom **Power Query-Editor** geladen und präsentiert werden. Die ursprüngliche Datenquelle ist im Gegensatz zu dieser bestimmten Ansicht der Daten, die angepasst oder *strukturiert* wird, nicht betroffen.

Die von Ihnen angegebenen Schritte (z.B. Tabelle umbenennen, Datentyp transformieren oder Spalten löschen) werden vom **Power Query-Editor** aufgezeichnet. Jedes Mal, wenn sich diese Abfrage mit der Datenquelle verbindet, erfolgen diese Schritte so, dass die Daten immer wie von Ihnen angegeben strukturiert werden. Dieser Vorgang erfolgt immer bei Verwendung der Abfrage in Power BI Desktop oder für jeden, der Ihre freigegebene Abfrage verwendet, z.B. im **Power BI**-Dienst. Diese Schritte werden im Bereich **Power Query-Einstellungen** unter **Angewendete Schritte** sequenziell erfasst.

Die folgende Abbildung zeigt den Bereich **Abfrageeinstellungen** für eine Abfrage, die bereits strukturiert ist. In den nächsten Abschnitten werden wir jeden dieser Schritte durchgehen.

![Fertige Abfrageeinstellungen](../media/pbid-clean-xform_01.png)

Kehren wir zurück zu den Daten für Pensionäre, die wir über die Verbindung mit einer Webdatenquelle gefunden haben. Lassen Sie uns nun die Daten so strukturieren, dass sie unseren Anforderungen entsprechen.

Für Einsteiger: Die meisten Bewertungen wurden in den **Power Query-Editor** als ganze Zahlen aufgenommen, aber nicht alle (eine Spalte enthielt Text und Zahlen, weshalb sie nicht automatisch konvertiert wurde). Power BI erkennt diese Änderungen häufig und führt automatisch den Schritt zum Ändern des Datentyps aus. 

Wir benötigen die Daten als Zahlen. Kein Problem: Klicken Sie einfach mit der rechten Maustaste auf die Spaltenüberschrift, und wählen Sie zum Ändern des Datentyps **Typ ändern > Ganze Zahl** aus. Wenn wir mehr als eine Spalte auswählen müssen, können wir zuerst eine Spalte auswählen, dann die **UMSCHALTTASTE** drücken und gedrückt halten, weitere benachbarte Spalten auswählen und dann mit der rechten Maustaste auf eine Spaltenüberschrift klicken, um alle ausgewählten Spalten zu ändern. Bei gedrückter **STRG-Taste** können wir auch nicht benachbarte Spalten auswählen.

![Fertige Abfrageeinstellungen](../media/pbid-clean-xform_02.png)

> Hinweis: Power Query erkennt oft, dass eine Textspalte aus Zahlen bestehen sollte, und ändert automatisch den Typ für Sie, wenn Sie die Tabelle in den Power Query-Editor übertragen. Wenn dies der Fall ist, gibt es in **Anwendete Schritte** eine Einstellung, die angibt, was Power Query für Sie durchgeführt hat.

Sie können den Typ dieser Spalten auch auf dem Menüband **Transformieren** von Text in Überschrift ändern bzw. *transformieren*. Hier ist das Menüband **Transformieren** mit einem Pfeil, der auf die Schaltfläche **Datentyp** zeigt. Sie ermöglicht Ihnen, den aktuellen Datentyp in einen anderen zu transformieren.

![Das Menüband „Transformieren“ und der Datentyp](../media/pbid-clean-xform_02b.png)

Beachten Sie, dass in **Abfrageeinstellungen** die vorgenommenen Änderungen unter **Angewendete Schritte** übernommen wurden. Wenn ich einen Schritt aus dem Strukturierungsprozess entfernen möchten, wähle ich diesen Schritt einfach aus und klicke dann links neben dem Schritt auf das **X**.

![Fenster „Abfrageeinstellungen“](../media/pbid-clean-xform_03.png)


## <a name="connect-to-data"></a>Herstellen einer Verbindung mit Daten
Diese Daten über verschiedene US-Bundesstaaten sind interessant und für zusätzliche Analyseaktivitäten und Abfragen nützlich. Doch es gibt ein Problem: Bei den meisten Daten wird ein Kürzel aus zwei Buchstaben für US-Bundesstaatcodes verwendet, nicht der vollständige Name des US-Bundesstaats. Wir benötigen eine Möglichkeit, Bundesstaatsnamen mit ihren Kürzeln zu verknüpfen.

Wir haben Glück: Es gibt eine andere öffentliche Datenquelle, die genau diese Aufgabe erfüllt. Aber es bedarf einer gewissen Strukturierung, bevor wir sie mit unserer Pensionärstabelle verbinden können. Unter dem folgenden Link finden Sie die Webquelle mit den US-Bundesstaatskürzeln:

<http://en.wikipedia.org/wiki/List_of_U.S._state_abbreviations>

Wählen Sie im **Power Query-Editor** auf dem Menüband auf der Registerkarte **Start** die Optionen **Neue Quelle > Web** aus. Geben Sie die Adresse ein, und klicken Sie auf **OK**. Im Fenster **Navigator** werden anschließend die auf dieser Webseite gefundenen Ergebnisse angezeigt.

![Von Website abgerufene Kürzel der US-Bundesstaaten](../media/pbid-clean-xform_04.png)

Wählen Sie **Codes and abbreviations...** aus, da diese Tabelle die gewünschten Daten enthält. Sie muss aber noch so strukturiert werden, dass sie nur noch die gewünschten Daten enthält. Gehen Sie dafür so vor:

Wir klicken auf **OK**, um die Daten in den **Power Query-Editor** zu übertragen und anschließend zu strukturieren. Fahren Sie dann so fort:

* *Entfernen Sie die ersten drei Zeilen*, die sich aufgrund der spezifischen Erstellung der Tabelle der Webseite ergeben haben und die wir nicht benötigen. Wählen Sie dazu im Menüband auf der Registerkarte **Start** zuerst **Zeilen entfernen** und dann im unteren Menü **Erste Zeilen entfernen** aus. Geben Sie in dem angezeigten Dialogfeld, in dem Sie gefragt werden, wie viele Zeilen entfernt werden sollen, **3** ein.

    ![Erste Zeilen entfernen](../media/pbid-clean-xform_04a.png)

* *Entfernen Sie die letzten 26 Zeilen*, die alle zu Gebieten gehören, die wir nicht einbeziehen möchten. Der Prozess ist identisch, aber dieses Mal wählen Sie **Untere Zeilen entfernen** aus und fügen 26 als die Anzahl der Zeilen ein, die entfernt werden sollen.

    ![Untere Zeilen entfernen](../media/pbid-clean-xform_04b.png)
<!-- -->
* *Filtern Sie Washington, D.C. heraus*. Die Tabelle mit den Statistiken für Pensionäre enthält diesen Bundesstaat nicht, weshalb wir ihn aus unserer Liste entfernen können. Klicken Sie dazu auf den Dropdownpfeil neben der Spalte *Name and status of region2*, und deaktivieren Sie dann das Kontrollkästchen neben „Federal state“. 

    ![Entfernen einer Zeile, die einen bestimmten Wert enthält](../media/pbid-clean-xform_04c.png)
<!-- -->

* *Entfernen Sie mehrere überflüssige Spalten*. Wir brauchen nur die Zuordnung des Bundesstaats zu seinem offiziellen Kürzel aus zwei Buchstaben, weshalb wir die anderen Spalten entfernen können. Wir behalten nur die zweite und fünfte Spalte. Wählen Sie dazu die erste zu löschende Spalte und dann bei gedrückter STRG-TASTE die anderen zu löschenden Spalten aus (so können Sie mehrere nicht zusammenhängende Spalten auswählen). Wählen Sie auf dem Menüband auf der Registerkarte „Start“ zunächst „Spalten entfernen“ und dann nochmals „Spalten entfernen“ aus.

    ![Entfernen bestimmter Spalten](../media/pbid-clean-xform_04d.png)
<!-- -->

* *Verwenden Sie die erste Zeile als Überschrift*. Da wir die ersten drei Zeilen entfernt haben, wird die aktuelle oberste Zeile zur gewünschten Überschrift. Klicken Sie einfach auf die Schaltfläche **Erste Zeile als Überschriften verwenden**.

    ![Erste Zeile als Überschriften verwenden](../media/pbid-clean-xform_04e.png)

    >[!NOTE]
    >An dieser Stelle sei darauf hingewiesen, dass die *Reihenfolge* der im **Power Query-Editor** angewendeten Schritte wichtig ist und sich auf die Strukturierung der Daten auswirken kann. Berücksichtigt werden muss auch, wie sich ein Schritt auf einen anderen, nachfolgenden Schritt auswirkt. Wenn Sie also aus **Angewendete Schritte** einen Schritt entfernen, verhalten sich nachfolgende Schritte wegen des Einflusses der Schrittreihenfolge der Abfrage ggf. nicht mehr so wie ursprünglich beabsichtigt.

* *Benennen Sie die Spalten und die Tabelle selbst um*. Wie üblich gibt es mehrere Möglichkeiten, eine Spalte umzubenennen, von denen Sie sich die bevorzugte aussuchen können. Lassen Sie uns die Spalten *State Name* und *State Code* umbenennen. Um die Tabelle umzubenennen, geben Sie einfach im Bereich **Abfrageeinstellungen** den Namen in das Feld **Name** ein. Wir nennen diese Tabelle **StateCodes**.

    ![Umbenennen von Spalten](../media/pbid-clean-xform_04f.png)

## <a name="combine-data"></a>Kombinieren von Daten

Nachdem wir nun die Tabelle *StateCodes* strukturiert haben, können wir die beiden Tabellen bzw. Abfragen kombinieren. Da die Tabellen, die wir jetzt haben, das Ergebnis der Abfragen sind, die wir auf die Daten angewendet haben, werden sie häufig auch als *Abfragen* bezeichnet.

Zum Kombinieren von Daten gibt zwei bevorzugte Möglichkeiten: *Zusammenführen* und *Anfügen*.

Wenn eine oder mehrere Spalten zu einer anderen Abfrage hinzugefügt werden sollen, werden die Abfragen **zusammengeführt**. Wenn einer vorhandenen Abfrage zusätzliche Datenzeilen hinzugefügt werden sollen, wird die Abfrage **angefügt**.

In diesem Fall möchten wir Abfragen zusammenführen. Zum Einstieg wählen wir die Abfrage aus, *mit der* die andere Abfrage zusammengeführt werden soll. Anschließend klicken wir auf dem Menüband auf der Registerkarte **Start** auf **Abfragen zusammenführen**. Wir wählen zuerst unsere Abfrage von Pensionärsdaten aus. Wenn wir schon mal dabei sind, benennen wir diese Abfrage in **RetirementStats** um.

![Schaltfläche „Abfragen zusammenführen“](../media/pbid-clean-xform_05.png)

Im eingeblendeten Fenster **Zusammenführen** werden wir aufgefordert, die Tabelle auszuwählen, die mit der ausgewählten Tabelle zusammengeführt werden soll. Anschließend müssen wir die Spalten angeben, die für die Zusammenführung verwendet werden sollen. 

Wählen Sie *State* in der Tabelle (Abfrage) *RetirementStats* und dann die Abfrage *StateCodes* aus. (Das ist in diesem Fall einfach, da es nur eine andere Abfrage gibt. Wenn Sie Verbindungen mit vielen Datenquellen herstellen, stehen hier viele Abfragen zur Auswahl.) Wenn Sie die übereinstimmenden Spalten (*State* aus *RetirementStats* und *State Name* aus *StateCodes*) richtig auswählen, sieht das Fenster **Zusammenführen** wie folgt aus, und die Schaltfläche **OK** ist aktiviert.

![Fenster „Zusammenführen“](../media/pbid-clean-xform_06.png)

Am Ende der Abfrage wird eine neue Spalte namens **NewColumn** erstellt, die den Inhalt der Tabelle (Abfrage) enthält, die mit der vorhandenen Abfrage zusammengeführt wurde. Alle Spalten aus der zusammengeführten Abfrage werden auf die neue Spalte **NewColumn** reduziert. Sie können jedoch die Tabelle **erweitern** und gewünschte Spalten einbeziehen. Um die zusammengeführte Tabelle zu erweitern und auszuwählen, welche Spalten einbezogen werden sollen, klicken Sie auf das Symbol „Erweitern“ (Symbol ![Erweitern](../media/pbid-clean-xform_07.png)). Das Fenster **Erweitern** wird geöffnet.

![Fenster „Erweitern“](../media/pbid-clean-xform_08.png)

In unserem Fall benötigen wir nur die Spalte *State Code*, weshalb Sie nur diese Spalte auswählen und dann auf **OK** klicken. Wir deaktivieren das Kontrollkästchen **Ursprünglichen Spaltennamen als Präfix verwenden**, da wir den ursprünglichen Spaltennamen nicht benötigen. Wenn das Kontrollkästchen aktiviert bleibt, erhält die zusammengeführte Spalte den Namen *NewColumn.State Code* (zusammengesetzt aus dem ursprünglichen Spaltennamen bzw. *NewColumn*, einem Punkt und dem Namen der in die Abfrage eingefügten Spalte).

>[!NOTE]
>Möchten Sie ein wenig mit dem Einfügen der Tabelle *NewColumn* experimentieren? Sie können ein wenig experimentieren. Wenn Ihnen die Ergebnisse nicht gefallen, löschen Sie diesen Schritt einfach im Bereich **Abfrageeinstellungen** in der Liste **Angewendete Schritte**. Ihre Abfrage wird dann wieder in den Zustand vor Anwenden des Schritts **Erweitern** zurückversetzt. Auf diese Weise können Sie beliebig oft und solange experimentieren, bis die Erweiterung Ihren Vorstellungen entspricht.

Wir haben jetzt eine einzelne Abfrage (Tabelle), in der zwei entsprechend den Anforderungen strukturierte Datenquellen miteinander kombiniert sind. Diese Abfrage kann als Grundlage vieler weiterer interessanter Datenverbindungen dienen, z.B. für Statistiken zu Wohnkosten, demografischen Daten oder Beschäftigungsmöglichkeiten in den US-Bundesstaaten.

Um die Änderungen im **Power Query-Editor** zu übernehmen und sie in Power BI Desktop zu laden, wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Schließen und übernehmen**.

![Schließen und Übernehmen von Dateneinstellungen](../media/pbid-clean-xform_09.png)

Nun können Sie in Ihrem Modell mit den Daten arbeiten. Als Nächstes befassen wir uns mit dem Erstellen von Visuals für Ihren Bericht.

Im Moment haben wir genügend Daten, um in Power BI Desktop eine Reihe interessanter Berichte zu erstellen. Da dies ein Meilenstein ist, speichern wir diese Power BI Desktop-Datei und nennen sie **Erste Schritte mit Power BI Desktop**. Wählen Sie auf dem Menüband auf der Registerkarte **Start** den Befehl **Datei > Speichern** aus.

Prima. Weiter zur nächsten Einheit, in der wir einige interessante Visuals erstellen.
