# Space

## Gliederung
[1.Vorstellung](#vorst)<br>
[2.Ausführung](#1)<br>
[3.Probleme](#2)<br>
[4.Stundenverlauf](#3)<br>
[5.Quellen](#4)<br>


### Vorstellung<a name="vorst"></a>
Die App "Space" verbindet ein Soundboard mit einem Raumschiff-Spiel. Es gibt ein Hauptmenü von dem aus man zum Soundbord oder zum Spiel gelangen kann. Das Soundboard besteht aus 14 Buttons mit bekannten Sätzen und Melodien aus Star Wars. Diese sind beschriftet, spielen bei Berührung den jeweiligen Soundtrack vollständig ab, oder stoppen diesen bei einer zweiten Berührung. Mit dem Menü-Button kann man zum hauptmenü zurückkehren. Bei dem Raumschiff-Spiel befindet sich ein Raumschiff am unteren rand, welches man mit der rechten und linken Pfeiltaste steuern kann. Mit der oberen Pfeiltaste kann das Raumschiff schießen. Am oberen Bildschirmrand bewegt sich ein zweites kleineres Raumschiff von links nach rechts, welches man versuchen muss zu treffen. Oben in der rechten Ecke befindet sich ein Button, mit dem das Spiel pausiert werden kann. Es eröffnet sich die Möglichkeit das Spiel weiter zu spielen, oder zum Hauptmenü zurück zu kehren.

### <a name="1"></a>Ausführung
Zum Programmieren der App wurde die Online-IDE App Lab von https://code.org/ verwendet. Sie dient dazu ohne viel Vorkenntnisse einem das Programmieren einer App nahezubringen. Um nun sowohl ein Spiel als auch ein Soundboard zu erstellen, muss die Option <b>Entwurf</b> angewählt werden. 

  (image/10-09-2018_1.png.jpg "Screenshot AppLab")

Dort können nun ganz einfach per Drag&Drop-Verfahren neue Bildschirme bzw. Screens erstellt werden. Selbiges gilt auch für die Knöpfe, welche dort, wie auch die Bildschirme, direkt editiert werden können. Wurde jedem Knopf und Bildschirm eine passende ID zugewiesen, so kann die Option <b>Code</b> angewählt werden. Hier kann man nun entscheiden, ob Bausteine oder Text verwendet werden soll, wobei sich auch bausteine in das Textformat bewegen lassen. Mit Hilfe des Bausteins <ins>onEvent("id", "click", function(event) { });</ins> lässt sich nun einer Aktion, bei dem ausgewählten Objekt, eine Reaktion zuweisen. Beispielsweise soll bei Druck des Knopfes <b>"Soundboard"</b> der Bildschirm auf <b>"Buttons"</b> geändert werden: onEvent("Soundboard", "click", function(event) {setScreen("Buttons"); }); <br> Um nun das Spiel programmieren zu können mussten einige Funktionen definiert werden, welche im Verlauf des Spiels aufgerufen werden. So musste für den Fall, dass das Schiff, welches gesteuert wird, den sichtbaren Beriech des Bildschirms verlässt, eine Funktion entwickelt werden, welche das Schiff auf die andere Seite des sichtbaren Bereiches ruft. Hierzu wurde gesagt, dass sobal die Position des Schiffes dazu tendiert zu verschwinden sie zurück auf die andere Seite gesetzt wird. Ebenfalls musste die Möglichkeit gegeben sein, dass man von der Position des Schiffes aus einen Schuss abfeuert, und dieser fliegt. Dies Wurde in zwei Funktionen unterteilt, da es zwei unterschiedliche Probleme behantelt. Einerseits das Positionieren vor dem Schiff zum anderen das bewegen. Zu letzt musste der gegner sich bewegen können und zerstört werden können. Auch hier für wurden zwei Funktionen angefertigt.

### <a name="2"></a>Probleme
Jedoch kam es bei der Codierung der Bewegung des Gegenrs und der Möglichkeit selbigen zu treffen Probleme. Diese beruhen vermutlich auf Logikfehlern im Code, welche sich auch nach mehr stündigem Überlegen nicht finden ließen. Dies hatte zu Folge, dass die Bewegung des Gegeners nur funtioniert, wenn sich etwas anderes auf dem Bilschirm bewegt. Diese Bewegung wird bei wiederholter Seitwärtsbewegung des eigenen Raumschiffs beschleunigt. Außerdem lässt sich der Gegner weder treffen, noch kann man ihn zerstören.

### <a name="3"></a>Stundenverlauf
Die ersten Stunden des Informatik Unterrichts haben wir damit verbracht die verschidenen zur Verfügung gestellten Programme auszuprobieren und uns mit den eventuellen Möglichkeiten auseinander zu setzten. Am <ins>10.09.2018</ins> habe wir uns dann dazu entschiden eine App zu programmiern. Außerdem waren wir uns ebenfalls schnell klar, dass diese auf jeden Fall ein Soundboard enthalten sollte. Hierzu schauten wir uns auf Youtube an, wie man in App Lab Sounds abspielt. Am nächsten Tag wurde uns kalr, dass ein Soundboard nicht ausreichen würde und so entschlossen wir uns dazu noch ein Spiel hinzu zu fügen. Auf Grund dessen, dass wir bereits etwas über die Möglichkeiten von App Lab recherchiert hatten, kamen wir zu dem Entschluss ein Space Invasion ähnliches Spiel zu programmieren. Dann haben wir nach und nach das Spiel programmiert. Irgendwann konnte man das Raumschiff bewegen, dann damit schiessen und zu letzt kam der Versuch den Gegner zu bewegen und treffen zu können.

### <a name="4"></a>Quellen
https://github.com/ThoreUndJonathan/InformatikUnterricht<br>
https://www.youtube.com/watch?v=jqAzVbpwRtE<br>
https://www.youtube.com/watch?v=SGQayvro64w
