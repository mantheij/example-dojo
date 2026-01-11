# Projektübersicht: Anti-Reversing

**Mitglieder:**

* Jan Manthei (215446)

## Der Rote Faden

Die Challenge führt in grundlegende Anti-Debugging-Techniken ein. Zuerst wird erkannt, dass das Programm unter einem Debugger nicht normal läuft. Danach wird die konkrete Debugger-Erkennung (TracerPid) identifiziert und analysiert. Anschließend wird diese Prüfung gezielt umgangen, um das Programm vollständig auszuführen. Ziel ist es, das Prinzip von Anti-Reversing zu verstehen und einfache Schutzmechanismen logisch auszuhebeln. Die Abfolge ist sinnvoll, da sie von Erkennen über Analyse bis zur Umgehung führt.

## Übersicht der Challenges

| Nr. | Titel der Challenge | Autor | Schwierigkeit (1-5) | Lernziel (Stichwort) |
| --- | ------------------- | ----- | ------------------- | -------------------- |
| 1   | Anti-Debug: TracerPid | Jan Manthei | ⭐ | Debugger-Erkennung erkennen und umgehen |

---

## Challenge starten

1. Öffne die Challenge in pwn.college.
2. Starte die Umgebung über den Start‑Button.
3. Warte, bis dir ein Terminal angezeigt wird.
4. Führe das Programm aus:

   ```bash
   ./run.sh
   ```
5. Analysiere das Verhalten des Programms und arbeite auf das Flag hin.
