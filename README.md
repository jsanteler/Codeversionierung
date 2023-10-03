# Codeversionierung


#Hier wurde ein Beispielablauf für Github FLow dokumentiert und festgehalten. Es wurde auf dem Repository FSEGitTest gearbeitet.


Riccardo hat ein GIT Repository erstellt.
Anschließend eine Java Datei erstellt und eine Nachricht platziert. Zusätzlich wurde ein Commit hinterlassen

```
git add Dateiname
git commit -m "Commit nachricht"
```

Diese wurde anschließend auf origin main gepusht.

```
git push
```

Danach wurde Branch "Julian" erstellt und julian hat das Repository auf sein Gerät geklont. Zum klonen wurde ein HTTPS Link verwendet

```
git clone URL
```

Branch Riccardo wurde Online erstellt und Riccardo hat auf diesen Branch mit seiner Dateiversionen gewechselt.

```
git checkout Riccardo - auf Riccardos Gerät
git checkout Julian - auf Julians Gerät
```

Julian hat in seinem Branch eine Änderung (zusätzliche Nachricht hinzugefügt) und diese Änderungen auf origin main gepusht.

Riccardo hat in seinem Branch eine Änderung gemacht ohne von den Änderungen von Julian zu wissen und wollte diese Änderungen auf den origin main mergen.
Dabei ist ein Konflikt entstanden.

Riccardo hat einen neuerlichen

```
git pull

```

durchgeführt und hat die Datei mit dem Konflikt heruntergeladen.
Nachdem der Konflikt aufgelöst (Code wurde in IDE zum laufen gebracht)
wurde konnte der merge auf origin main durchgeführt werden.

Nachdem der Konflikt gelöst wurde konnten wir online mit "Open pull Request" die "Julian Branch" zur main Branch mergen.

Anschließend wurde der Fehler von Julian erneut produziert um die Online Resolve Möglichkeit auszuprobieren.
Siehe Commits

**GitHub Flow Vor und Nachteile**

_Vorteile_

- Klarheit: Durch die direkte Struktur von GitHub Flow ist es leicht zu begreifen, besonders vorteilhaft
für kleinere Gruppen.

- Schnelle Codeanpassung möglich

- Der gesamte Entwicklungszyklus ist verfolgbar und nachvollziehbar.

_Nachteile_

- Bei größerer Anzahl an Mitwirkenden kann die Übersicht verloren gehen. Nicht optimal für umfangreiche Projekte.

- Schnelle Änderungen kann zu Fehler führen und kollisionen verursachen.

- Für sehr große Softwareentwicklungsprojekte nicht optimal.


**Andere Codeversionierungsstrategien**


Auf der Suche nach weiteren Strategien bin ich auf Gitflow Workflow gestoßen.
Gitflow verwendet verschiedene Branch-Typen wie Master, Develop, Feature, Release und Hotfix. 
Dies ermöglicht es Teams, gleichzeitig an verschiedenen Features und Releases zu arbeiten, indem sie klare Branch-Strukturen verwenden.

Noch dazu hab ich etwas über Trunk Based Development gelesen.
In dieser Strategie arbeitet das gesamte Team direkt im Hauptbranch. Es gibt keine Feature-Branches.
Stattdessen werden Änderungen häufig und in kleinen Mengen eingecheckt. Dieser Ansatz erfodert viel Disziplin.