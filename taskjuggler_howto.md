# Howto taskjuggle..

Für das Projekt Management verwenden wir TaskJuggler. Damit werden die Informationen auf https://fablabnbg.github.io/Umzug/ anhand der Projektkonfiguration auf https://github.com/fablabnbg/Umzug generiert.

Für die einzelnen Bereiche ("Teilprojekte") haben wir Verantwortliche festgelegt.

## Helfer

Zur Planung benötigen wir folgende Informationen:
  * Wann Ihr üblicherweise Zeit habt, prinzipiell dem Lab zu helfen.
    * Als Standard haben wir "Mo - Fr 18:00 - 22:00 und Sa - So 10:00 - 22:00" festgelegt.
  * Wann ihr nicht zur Verfügung steht (Urlaub wegfahren, Dienstreisen usw.) oder besonders viel zur Verfügung steht (Urlaub zu Hause)
  * Aktuelle Kontaktdaten (Mail und Handy)
  * Wieviel Zeit (in Stunden) ihr ungefähr pro Woche oder Monat für den Lab-Umzug habt
    * z.B. "20h", wenn 2 Abende unter der Woche a 5 Stunden und ein Tag am Wochenende a 10h möglich sind.

## Verantwortliche

### ... like a n00b

Überlegt euch, in welche Aufgaben ihr euren Bereich unterteilt. Aufgaben sind:

* Alles, wofür Ihr Helfer braucht (pro "Aktion" eine Aufgabe)
* Alles, was als Vorbereitung für eine andere Aufgabe dient (z.B. Planung oder Reservierung von zu leihenden Geräten)
* Thematisch zusammenhängende Aufgabe sollen durch eine übergreifene Aufgabe gruppiert werden

Überlegt euch, was Grundvorraussetzung ist, damit die Aufgabe starten kann

* Es sollte genau einer der definierten Meilensteine Grundvorraussetzung sein (z.B. "Rohbau fertig").  
* In der Regel bauen die Aufgaben innerhalb eines Verantwortungsbereich aufeinander auf, es sollte klar erkenntlich sein, wie.
* Abhängigkeiten zu Aufgaben anderer Bereiche sind auch möglich, sollten aber so gering wie möglich gehalten werden.
  * wenn möglich, sollten stattdessen die Meilensteine verwendet werden
* Wenn Wartezeiten dabei sind (z.B. Bestellungen, Reservierung Werkzeug) plant diese mit genügend Puffer ein

* __TODO__: Template Aufgabe

Überlegt euch, wie groß der Aufwand ist, die Aufgabe durchzuführen

* Angabe in Personenstunden
* Wieviel Helfer (inkl. euch selbst) benötigt ihr sinnvollerweise? (Wieviel mindestens, wie viel sind es sinnvollerweise maximal?)


### ... like a pro

* macht euch die gleichen Überlegungen wie die n00bs ;-)
* .. aber tragt die Daten selbst in die taskjuggler-Datei (.tji) für Euren Bereich ein.

#### Vorraussetzung

* Schreib-Zugriff auf fablabnbg github-Repositories
* Sinnvollerweise eine lokale taskjuggler-Installation, um Änderungen zu testen

#### Grundlagen

* Ihr definiert die Aufgaben mit dem Schlüsswort `task`
* Abhängigkeiten werden mit `depeneds` definiert.
* Den Gesamtaufwand in Personenstunden gibt ihr mit `effort` an. Falls ein Task andauert, aber keinen Aufwand erzeugt (z.B. Trockenzeiten), gebt eine Duration an.
* Die benötigten Ressourcen (Helfer, aber auch Werkzeug) gibt ihr mit `allocate` an.
* Die vorhandenen Ressourcen seht ihr in der Datei [Resourcen.tji](https://github.com/fablabnbg/Umzug/blob/master/Resourcen.tji)
* Um Helfer aus den Pool zu allozieren, nutzt das Makro `${select1FromHelperPool}`

#### Details Aufgaben

* __TODO__

#### Details Ressourcen

* __TODO__
* Wartezeiten:
  * wenn diese Ressourcen binden (z.B. Lab oder Bereiche vom Lab): als Task mit einer festen `duration` eintragen (z.B. Boden trocknet nach Streichen)
  * wenn diese keine Ressourcen binden (z.B. Bestellung): Nutzt Abhängigkeiten mit einer `mingapduration`.
