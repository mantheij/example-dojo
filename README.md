# Gruppen-Manifest: [Anti-Reversing]

**Mitglieder:**

* Jan Manthei (215446)

## Der Rote Faden

*Die Challenge führt Studierende in Anti-Debugging-Techniken ein. Zuerst erkennen sie, dass ein Programm unter Debuggern blockiert wird. Dann lernen sie, wie man die Debugger-Erkennung (TracerPid) identifiziert und analysiert. Anschließend üben sie, den Check zu umgehen, ohne das Programm zu zerstören. Ziel ist, dass sie verstehen, wie Anti-Reversing funktioniert und warum Programme Schutzmechanismen einsetzen. Die Reihenfolge ist sinnvoll, weil sie von Erkennen → Analysieren → Umgehen geht. So baut jeder Schritt auf dem vorherigen auf, ohne dass Wissen übersprungen wird. Am Ende können Studierende selbstständig ähnliche Schutzmaßnahmen verstehen und testen.*

## Übersicht der Challenges

| Nr. | Titel der Challenge | Autor | Schwierigkeit (1-5) | Lernziel (Stichwort) |
| --- | ------------------- | ----- | ------------------- | -------------------- |
| 1   | Debugger Detection         | Jan   | ⭐                   | Anti Reversing umgehen            |

---

# Verwendung von `daddel`

`daddel` kann über den folgenden `docker`-Befehl gestartet werden:

```bash
docker run -it --network host \
  -v "$(pwd):/challenge" \
  ghcr.io/s-solom/daddel:dev \
  --config /challenge/my-config.yml --debug
````

* `--config`: Pfad zur Config-Datei **relativ zum aktuellen Verzeichnis**, da `$(pwd)` nach `/challenge` gemountet wird.
  Beispiel: `examples/dynamic.config.yml` muss lokal unter `./examples/dynamic.config.yml` existieren.
* `--debug`: Aktiviert den Debug-Modus (hilfreich beim Entwickeln für detailiertere Ausgaben).

## Beispiele

Als erstes können die beiden Beispiel-Configs aus den Challenges getestet werden:

* **Static**: Config in `Challenge_01_static`
* **Dynamic**: Config in `Challenge_02_dynamic`

Für den **Dynamic**-Typ befindet sich der Code der Demo-App in `Challenge_02_dynamic/submission/src`.
