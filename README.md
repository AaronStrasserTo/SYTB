# OS - Prozesse
## Prozess Konzept
- Prozess -> Definition: Ein Prozess ist ein in Ausführung befindliches Maschinenprogramm. Es muss nicht zwingend aktiv sein.
- Wartezeiten auf Rückgaben in einzelnen Prozessen oder auch Modulen sollen vermieden werden.
- Beispiel: "Büroarbeitsplatz
- Prozesse sind in einem Betriebssystem ein zentrales Konzept um in der Interaktion aus vielen Prozessaufgaben und deren E/A-Operationen bestmögliche Effizienz zu gewährleisten.
- Während ein Maschinenprogramm nur eine Folge von Befehlen ist, so wird dieses Programm zum Prozess, indem es in den Speicher geladen wird, einen eigenen Kontext erhält und gestartet wird (Programmzähler auf Anfangsadresse des Maschinenprogramms setzen). Es ist in Ausführung.
- Adressierung Prozess
  - Aktueller Wert des Programmzählers
  - Aktuelle Werte der Register und Variablen

## Kontext
- Prozesskontext -> Ein Prozesskontext beinhaltet den aktuellen Systemzustand (Ausführungszustand). Er wird vollständig beschrieben. Dazu zählen unter anderem Prozessstatus-Informationen und CPU-Register Belegungen.
- Ein Prozess-Kontext beinhaltet alles, was man für eine Weiterführung eines unterbrochenen Prozesses benötigt, um diesen auf dem lokalen Computersystem fortsetzen zu können.

## Image
- Prozess-Image: Als Image eines Prozesses bezeichnet man die Gesamtheit der physischen Betandteile eines Prozesses, also insbesondere seine Befehlsfolge (Trace), aber auch seinen Kontext, lokale und globale Variablen und der Ausführungs-Stack.
- Zu einem Prozess-Image gehört alles, was man von einem unterbrochenen Prozess benötigt, um ihn auf ein anderes Computersystem zu transportieren und dort fortzusetzen.
- Prozess-Image = Prozess-Kontext + Programm + Stack

## Uniprogramming
- Beim Uniprogramming werden Prozesse sequenziell nacheinander, vollständig und ohne Unterbrechung ausgeführt.
  - Vorteile
    - Einfache Handhabung von Programmabläufen
    - Kein Management von parallelen Programmzuteilungen bezüglich Ressourcen notwendig
  - Nachteile
    - Ineffiziente Nutzung von Computing Ressourcen (CPU, RAM, etc.)
    - Erhöhte Wartezeiten
- Welches Problem ergibt sich, wenn jeder Prozess auf den vollständigen Abschluss des vorhergehends Prozess warten muss?
  - Diskussion mit Beispielen
