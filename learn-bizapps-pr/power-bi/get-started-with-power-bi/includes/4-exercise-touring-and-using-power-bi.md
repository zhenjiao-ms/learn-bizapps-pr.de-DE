Wie wir in der vorherigen Einheit gesehen haben, ist der allgemeine Arbeitsablauf in Power BI das Erstellen eines Berichts in Power BI Desktop, das Veröffentlichen des Berichts über den Power BI-Dienst und dessen anschließende Freigabe für andere Benutzer, damit diese ihn im Dienst oder in einer mobilen App anzeigen können.

Einige Benutzer beginnen Ihre Arbeit aber im Power BI-Dienst. Daher werfen wir einen kurzen Blick auf den Dienst, um eine einfache und beliebte Vorgehensweise kennenzulernen, mit der in Power BI schnell visuelle Elemente erstellt werden können: *Apps*.

Eine **App** ist eine Sammlung mit vorkonfigurierten, fertigen visuellen Elementen und Berichten, die für eine gesamte Organisation freigegeben werden. Die Verwendung einer App ist mit dem Zubereiten eines Fertiggerichts in der Mikrowelle oder dem Bestellen eines Fastfood-Menüs vergleichbar: Nach wenigen Klicks und Eingaben erhalten Sie in kurzer Zeit eine Zusammenstellung von Speisen, die gut zusammenpassen und in einer sauberen und bequemen Verpackung geliefert werden.

Wir sehen uns daher kurz die Apps, den Dienst und die Funktionsweise an. In den nächsten Modulen werden Apps (und der Dienst) ausführlicher behandelt. Sie können sich dieses als Appetithäppchen vorstellen.

## <a name="create-out-of-the-box-dashboards-with-cloud-services"></a>Erstellen von Standarddashboards mit Clouddiensten
Mit Power BI ist es einfach, eine Verbindung mit Daten herzustellen. Im Power BI-Dienst können Sie auf der Startseite unten links einfach die Schaltfläche **Daten abrufen** wählen.

![Power BI-Dashboards](../media/pbi-touring_01.png)

Auf dem *Canvas* (mittlerer Bereich des Power BI-Diensts) werden die verfügbaren Datenquellen im Power BI-Dienst angezeigt. Zusätzlich zu allgemeinen Datenquellen wie Excel-Dateien, Datenbanken oder Azure-Daten kann mit Power BI genauso leicht auch eine Verbindung mit **Softwarediensten** (auch als SaaS-Anbieter oder Clouddienste bezeichnet), z.B. Salesforce, Facebook oder Google Analytics, und vielen anderen SaaS-Diensten hergestellt werden.

![Power BI – Daten abrufen](../media/pbi-touring_02.png)

Für diese Softwaredienste stellt der **Power BI-Dienst** eine Sammlung mit einsatzbereiten visuellen Elementen bereit, die in Dashboards und Berichten für Ihre Organisation vorab angeordnet sind (und als **Apps** bezeichnet werden). Mit Apps können Sie in Power BI schnell mit Daten und Dashboards arbeiten, die Ihre Organisation für Sie erstellt hat. Bei Verwendung der GitHub-App stellt Power BI beispielsweise eine Verbindung mit Ihrem GitHub-Konto her (nach Angabe Ihrer Anmeldeinformationen) und füllt dann eine vordefinierte Sammlung mit visuellen Elementen und Dashboards in Power BI mit Daten.

Es gibt Apps für alle möglichen Onlinedienste. Die folgende Abbildung zeigt einen Bildschirm mit Diensten, die bei verschiedenen Onlinediensten verfügbar sind, in alphabetischer Reihenfolge. Dieser wird angezeigt, wenn Sie im Feld **Dienste** die Option **Abrufen** wählen (siehe die vorherige Abbildung). Wie Sie in der folgenden Abbildung sehen, können Sie unter vielen Diensten wählen.

![Power BI-Dienste](../media/pbi-touring_03.png)

Für unsere Zwecke wählen wir **GitHub**. GitHub ist eine Anwendung für die Online-Quellcodeverwaltung. Wenn ich jetzt in der GitHub-App auf **Jetzt anfordern** klicke, wird das Fenster **Mit GitHub verbinden** angezeigt. 

![Die GitHub-App](../media/pbi-touring_03b.png)

Nach Eingeben der Informationen und Anmeldeinformationen für die GitHub-App wird mit der Installation der App begonnen.

![Importieren von Daten](../media/pbi-touring_04.png)

Nach dem Laden der Daten wird das vordefinierte GitHub-App-Dashboard angezeigt.

![Geladene Power BI-App](../media/pbi-touring_05.png)

Zusätzlich zum **Dashboard** der App ist auch der **Bericht** verfügbar, der für die Erstellung des Dashboards generiert wurde (als Teil der GitHub-App). Dies gilt auch für das **Dataset** (Sammlung mit Daten aus GitHub), das während des Datenimports erstellt und zum Erstellen des GitHub-Berichts verwendet wurde.

![Power BI-Navigation](../media/pbi-touring_06.png)

Auf dem Dashboard können Sie auf eines der Visuals klicken und mit ihnen interagieren, woraufhin alle anderen Visuals auf der Seite reagieren. Wenn im Visual **Pull Requests (by month)** beispielsweise auf den Balken **May 2018** geklickt wird, passen sich die anderen Visuals auf der Seite an diese Auswahl an.

![Power BI-Navigation](../media/pbi-touring_06b.png)

## <a name="refreshing-data-in-the-power-bi-service"></a>Aktualisieren von Daten im Power BI-Dienst
Sie können das Dataset für eine App oder andere Daten, die Sie in Power BI nutzen, auch **aktualisieren**. Um Aktualisierungseinstellungen festzulegen, klicken Sie auf das Symbol für die Zeitplanaktualisierung für das Dataset, das Sie aktualisieren möchten. Ein Menü wird eingeblendet. Sie können auch auf das Aktualisierungssymbol daneben (den Kreis mit einem Pfeil) klicken, um es sofort zu aktualisieren.

![Planen der Aktualisierung für Dashboards](../media/pbi-touring_09.png)

Die Registerkarte **Datasets** wird im eingeblendeten Einstellungsfenster ausgewählt. Klicken Sie auf den Pfeil **Zeitplanaktualisierung**, um diesen Abschnitt im rechten Fensterbereich zu erweitern. Das Dialogfeld „Einstellungen“ wird auf der Canvas angezeigt, damit Sie die gewünschten Aktualisierungseinstellungen vornehmen können.

![Schaltflächen für das Planen der Aktualisierung](../media/pbi-touring_10.png)

Dies soll als kurze Übersicht über den Power BI-Dienst reichen. Es gibt in Bezug auf den Dienst noch viele weitere Möglichkeiten, die später in diesem und weiteren Modulen beschrieben werden. Beachten Sie auch, dass Sie Verbindungen mit vielen unterschiedlichen Arten von Daten herstellen und viele verschiedene Apps nutzen können. Außerdem werden ständig weitere Apps hinzugefügt.

