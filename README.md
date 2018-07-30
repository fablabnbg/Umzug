# Projektplanung Umzug

Die Projektplanung für den Umzug wird mit
[TaskJuggler](http://taskjuggler.org) gemacht, ein einfaches,
[Ruby](https://www.ruby-lang.org)-basiertes Werkzeug zur Verwaltung
von Terminen, Aufgaben und deren Abhängigkeiten.

## Aktueller Projektstand

https://fablabnbg.github.io/Umzug/


## Benutzung

1. TasjJuggler installieren (`gem install taskjuggler`)

2. Dieses Repo clonen (`git clone https://github.com/fablabnbg/Umzug.git`)

3. `rake`


### Aufwände eintragen

* Festes Datum

  `start` &lt;datum&gt; und `end` &lt;datum&gt; verwenden

  oder

  `start` &lt;datum&gt; `+`&lt;n&gt;`d` für 'n' Tage

* Feste Länge, egal wieviel Helfer

  `length`

* Skaliert auf mehr Helfer

  `effort`


## Travis CI

Letzter Build [hier](https://travis-ci.org/fablabnbg/Umzug)


## Styleguide

* Zeilenumbruchszeichen LF
* Einrückung mit 2 Leerzeichen je Ebene
* Leerzeichen am Zeilenende vermeiden
* IDs je nach Typ am Anfang mit a,t,r gefolgt von einem Unterstrich vergeben
