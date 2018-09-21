In der vorherigen Einheit haben wir zwei Datenquellen miteinander verbunden und diese Datenquellen nach unseren Vorstellungen strukturiert und kombiniert. Als Ergebnis verfügen wir nun über ein **Datenmodell**, das wir als Grundlage für die Erstellung von Berichten verwenden können. 

Das bedeutet nicht, dass wir für immer an diesem Datenmodell festhalten müssen. Änderungen können im Power Query-Editor vorgenommen werden, nachdem das Modell geladen wurde. Sie können auch ein Modell neu laden, um alle vorgenommenen Änderungen zu übernehmen. Aber vorerst reicht dieses Modell völlig aus. 

Um mit der Erstellung eines Berichts mit dem von uns erstellten Datenmodell zu beginnen, öffnen wir in Microsoft Power BI Desktop die Ansicht **Bericht**.

Die Ansicht **Bericht** hat fünf Hauptbereiche:

1. Das Menüband, auf dem gängige Aufgaben im Zusammenhang mit Berichten und Visualisierungen gezeigt werden
2. Die Ansicht **Bericht** bzw. den Zeichenbereich, in der/dem Visualisierungen erstellt und angeordnet werden
3. Den Registerkartenbereich **Seiten** im unteren Bereich, in dem Sie Berichtsseiten auswählen oder hinzufügen können
4. Den Bereich **Visualisierungen**, in dem Sie Visualisierungen ändern, Farben oder Achsen anpassen, Filter anwenden, Felder ziehen und vieles mehr können
5. Den Bereich **Felder**, in dem Abfrageelemente und Filter entweder in die Ansicht **Bericht** oder den Bereich **Filter** des Bereichs **Visualisierungen** gezogen werden können

![Bereiche der Ansicht „Bericht“](../media/pbid-visuals_01.png)

Die Bereiche **Visualisierungen** und **Felder** können durch Klicken auf den kleinen Pfeil am Rand ausgeblendet werden, wodurch in der Ansicht **Bericht** mehr Platz zur Erstellung überzeugender Visualisierungen zur Verfügung steht.

![Bereiche ausblenden](../media/pbid-visuals_02.png)

## <a name="create-visuals"></a>Erstellen von Visuals
Zum Erstellen einer Visualisierung ziehen Sie einfach ein Feld aus der Liste **Felder** auf die Ansicht **Bericht**. Ziehen Sie in diesem Fall das Feld **State** aus **RetirementStats**, und verfolgen Sie, was passiert.

![Ziehen eines Felds in den Zeichenbereich](../media/pbid-visuals_03a.png)

Wie Sie sehen, hat Power BI Desktop automatisch eine kartenbasierte Visualisierung erstellt, da die Software erkannt hat, dass das Feld **State** Daten zu geografischen Standorten enthält.

![Ein Kartenvisual](../media/pbid-visuals_03.png)

Beachten Sie, dass Sie im Bereich **Visualisierungen** verschiedene Arten von Visualisierungen auswählen können. Anschließend können Sie im Bereich unter diesen Symbolen Felder in verschiedene Bereiche ziehen, um eine Legende hinzuzufügen oder die Visualisierung auf andere Weise zu ändern. 

![Das erste Visual](../media/pbid-visuals_04.png)

Lassen Sie uns einige Visuals auf dieser ersten Berichtsseite erstellen, und sehen, was passiert.

Sie können den Typ eines Visuals ändern, indem Sie es einfach auf dem Zeichenbereich auswählen und im Bereich **Visualisierungen** eine andere Kachel auswählen. Das werden wir jetzt tun. Wählen Sie anstelle von **Karte** (Kachel mit Globussymbol) **Flächenkartogramm** (die nächste Kachel, die wie Bundesstaaten in verschiedenen Farben aussieht) aus.

**Erstes Visual**

Ziehen Sie das Feld **Overall rank** (Allgemeine Rangfolge) aus dem Bereich **Felder** im Bereich **Visualisierungen** in den Abschnitt **Farbsättigung**. 

![Anpassen des ersten Visuals](../media/pbid-visuals_04b.png)

Um die in der Karte verwendeten Farben anzupassen, wählen Sie die (wie eine Farbrolle aussehende) Registerkarte **Format** im Bereich **Visualisierungen** aus. Erweitern Sie dann **Datenfarben**, um die Farben anzupassen.

![Ändern von Datenfarben](../media/pbid-visuals_04c.png)

Sie können die Größe des Visuals anpassen, indem Sie seine Ecken oder Seiten ziehen. Lassen Sie uns dieses Visual nach links oben verschieben, bevor wir das nächste erstellen.

Wählen Sie einen leeren Bereich des Zeichenbereichs aus, sodass kein Visual ausgewählt ist. Sie sind jetzt bereit sind, Felder zu ziehen und das nächste Visual zu erstellen.

**Zweites Visual**

Ziehen Sie **State** aus **RetirementStats** in einen leeren Bereich des Zeichenbereichs. Ziehen Sie dann das Feld **Overall rank** (Allgemeine Rangfolge), danach das Feld **Health care quality** (Qualität des Gesundheitswesens) und das Feld **Well-being** (Gemeinwohl) auf dieses Visual. Nun ändern wir das Visual in den Typ **Linien- und gruppiertes Säulendiagramm**, indem wir im Bereich **Visualisierungen** die Kachel dieses Visuals auswählen.

Wir haben es fast geschafft. Verschieben Sie auf der Registerkarte **Felder**das Feld **Well-being** zu **Zeilenwerte**. Das folgende Bild zeigt, wie Ihr Visual nun aussehen soll. Beachten Sie, dass die Darstellung eines Visuals durch die Reihenfolge der Felder in den einzelnen Buckets verändert wird. Beispielsweise befindet sich **Health care quality** (Qualität des Gesundheitswesens) im Bucket **Column values** (Spaltenwerte) oberhalb von **Overall rank** (Allgemeine Rangfolge), wie in der folgenden Abbildung dargestellt. 

![Fertiges Visual](../media/pbid-visuals_04d.png)

Sie können mit diesen Visuals so viel experimentieren, wie Sie möchten: den Visualtyp ändern, Felder hinzufügen, Farben ändern oder es im Zeichenbereich anordnen. Alle diese Änderungen machen Spaß, lassen sich leicht rückgängig machen und sind schnell wirksam.

Wir machen mal einen Schnellvorlauf und sehen uns an, wie die Ansicht **Bericht** nach dem Hinzufügen einiger Visualisierungen und neuer Berichtsseiten aussieht. Keine Sorge, Sie können diesen Bericht aus erster Hand sehen. Die Einheit mit der Zusammenfassung dieses Moduls enthält einen Link zum Herunterladen der endgültigen PBIX-Datei. Sie können den Bericht in Ihre lokale Version von Power BI Desktop laden und genau erkennen, wie das Ergebnis zustande gekommen ist. 

Die erste Berichtsseite enthält eine Ansicht der Daten basierend auf *Overall Rank* (Allgemeine Rangfolge). Wenn Sie eine der Visualisierungen auswählen, wird im Bereich **Felder und Filter** angezeigt, welche Felder ausgewählt wurden. Ersichtlich ist auch die Struktur der Visualisierung (d.h. welche Felder auf **Gemeinsame Achse**, **Spaltenwerte** und **Zeilenwerte** angewendet wurden).

![Eine fertige Berichtsseite](../media/pbid-visuals_05.png)

In diesem Bericht gibt es sechs **Seiten**, auf denen jeweils bestimmte Datenelemente visualisiert werden:

1. Die erste Seite (siehe die Abbildung oben) enthält alle Bundesstaaten auf der Basis *Overall Rank* (Allgemeine Rangfolge).
2. Die zweite Seite konzentriert sich auf die 10 besten Bundesstaaten auf der Basis *Overall Rank* (Allgemeine Rangfolge).
3. Die dritte Seite zeigt die 10 besten Bundesstaaten in Bezug auf Lebenshaltungskosten (und die entsprechenden Daten).
4. Auf der vierten Seite steht das Wetter mit den 15 Bundesstaaten mit den meisten Sonnenstunden im Mittelpunkt.
5. Die fünfte Seite zeigt die 15 besten Bundesstaaten hinsichtlich des Gemeinwohls.
6. Die sechste Seite konzentriert sich auf Kriminalitätsstatistiken und zeigt die 10 besten und 10 schlechtesten Staaten.

Und so sieht die Seite mit dem Schwerpunkt auf den Lebenshaltungskosten aus.

![Ein fertiger Bericht](../media/pbid-visuals_06.png)

Es gibt viele interessante Berichte und Visualisierungen, die Sie erstellen können. Doch das Beste am Erstellen von Berichten ist, dass sie für andere freigegeben werden können. In der nächsten Einheit erfahren Sie, wie einfach das Freigeben von Power BI-Berichten ist.

## <a name="adding-report-pages"></a>Hinzufügen von Berichtsseiten

Alle Berichte verfügen anfänglich über mindestens eine leere Seite. Seiten werden im Navigationsbereich links neben dem Zeichenbereich angezeigt. 

Sie können einer Seite alle Arten von Visualisierungen hinzufügen, aber Sie sollten es nicht übertreiben. Zu viele Visualisierungen auf einer Seite führen zu einer Überfrachtung und erschweren das Auffinden der gewünschten Informationen.

Um dem Bericht eine Seite hinzuzufügen, klicken Sie einfach auf dem Menüband auf **Neue Seite** oder neben der letzten Berichtsseite auf das Pluszeichen **+**.

![Hinzufügen einer Berichtsseite](../media/pbid-visuals_09.png)

Selbst mit nur ein paar wenigen Visuals haben Sie nun einen Bericht. Lassen Sie uns zur nächsten Einheit übergehen und erfahren, wie wir diese mit Erkenntnissen gefüllten Berichte für andere freigeben können.