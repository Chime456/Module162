# Daten Analysieren und modellieren-Module162
Tag 1

**Markdown Tutorial**  
Heute haben wir die Einführung mit Gitlab bzw. Github. Da ich schwierigkeiten hatte mich bei Gitlab zu registrieren, habe ich mich stattdessen im Github angemeldet.
Danach fing es an mit der erster Auftrag welches das [Markdown Tutorial](https://www.markdowntutorial.com/de/) war.
Insgesamt sind es 8 Tutorials zu den Grundlagen wie man im Github & Gitlab programmiert.
* Kursiv- und Fettdruck
* Überschriften
* Links
* Bilder
* Blockquotes
* Listen
* Paragraphen
* Fazit  

Dazu konnte man die [Basic Syntaxe](https://www.markdownguide.org/basic-syntax/) nachschauen, was mehr theorie mit Beispiele enthaltet, welches mit der HTML vergliechen wird.

--------

# Strukturierte und unstrukturierte Daten  
Tag 2

To Do:
[Strukturierte und Unstrukturierte Daten](https://gitlab.com/ch-tbz-it/Stud/m162/-/blob/main/Daten_Formate/StrukturierteDaten.md?plain=0)  
**Was ist Datenstruktur**  
* Es ist ein Objekt zur Speicherung und Organisaiton
* Die Daten werden in bestimmen Art und Weise angeordnet und verknüpft, um den Zugriff auf Daten effizient zu ermöglichen

**Strukturierte und unstrukturierte Daten**
* Es legt das allgemeine Verhalten der Organisation fest
* Es handelt sich von

**Einordnung**

**Modellierung**

**Behandlung von unstrukturierten Daten**

**Organisation von Daten**

# Skala
### Skalentypen
**Diskret**:
Daten sind diskret, wenn es abzählbare Anzahl an möglichen Werten gibt  
**Stetig**:
Daten sind stetig, wenn es unendlich viele mögliche Werte gibt, die **nicht** abzählbar sind

**Nominalskala**: Mögliche Werte haben keine Rangordung, gleichwertig (Geschlecht)

**Ordinalskala**: steht in einer Rangordnung (Schulnoten)

**Kardinalskala**: Steht in einer Rangordnungund zueinander und Abstände sind gleichmässig 

**Intervallskala**: Rangordung und Abstände definiert, kein natürlihcer Nullpunkt (Temparatur)

**Verhältnisskala**: Rangordnung und Abstände definiert, nautürlicher Nullpunkt (Abstand in cm)

[Übersicht](https://gitlab.com/ch-tbz-it/Stud/m162/-/raw/main/Daten_Formate/images/Skalenniveaus.jpg) über die Kategorisierung

**Häufbarkeit**
Werte sind häufbar, wenn sie mehrfach vorkommen können.  
* **nicht Häufbar**:  
  Sie werden in einem Fragenbogen an der TBZ gefragt, welches ihr Lieblingsmodul ist.
  Durch die Fragestellung wird klar, dass sie nur ein Modul auswählen können. Typische andere
  Ausprägungen sind z.B. das Geschlecht oder Alter einer Person.
* **Häufbar**:  
  Sie werden in einem Fragebogen an der TBZ gefragt, welche Module sie im letzten
  Semester besuchten.
  Durch die Fragestellung wird klar, dass sie mehrere Module auswählen können

-------

# Datentypen
TAG 3, 01.09.2025

**Ganze Zahlen**   
BIGINT: 64 bit, Darstellung sehr großer Ganzzahlen gedacht  
BIN (Binary): bit ist felxibel, reiner Binärwert / Bitmuster, das man entweder als Zahl oder als Datenblock interpretiert.
INT: 
LONG:
SHORT:

**Natürliche Zahlen**   
NATURAL:
BYTE: 8 bit, kleinster ganzzahliger Speicherbereich, der für kleine Zahlen, Steuerwerte, Flags oder Rohdaten verwendet wird.  
CARDINAL: 16-32 bit, ganze Zahl ≥ 0, typischerweise 32 Bit, wird verwendet, wenn negative Zahlen nicht sinnvoll sind.

**Festkommazahlen (Dezimalzahlen)**   
COMP-3: bit ist flexibel, platzsparender, präziser Dezimal-Datentyp für Finanz- und Geschäftsanwendungen.  
CURRENCY: 64 bit, 64-Bit-Festkommazahl für Geldbeträge, die präzise Berechnungen ermöglicht, ohne dass Rundungsfehler auftreten.

**Aufzählungstypen**   
ENUM: ein Wert aus einer festen Liste  
SET/IMPLIZIT: mehrere Werte aus einer festen Liste gleichzeitig

**Boolean**   
BOOL:
BOOLEAN:

**Zeichen (einzelnes Zeichen)**   
CHAR:
CHARACTER:

**Gleitkommazahlen**   
DOUBLE:
FLOAT:

**Zeichenkette feste/variabler Länge**  
ARRAY:

**Datum & Zeit**  
DATE:
TIME:
DATETIME:
TIMESTAMP:

---------

# Auftrag: Datentypen

#### Aufgabe 1

Welche Datentypen könnten den folgenden Werten zugrunde liegen?

| Wert                                           | Datentype(n) |
| ---------------------------------------------- | ------------ |
| A                                              |  Zeichen      |
| 23                                             |  Ganz Zahl     |
| 12021.25                                       |  Dezimalzahl     |
| 0                                              |  Ganze Zahl   |
| Ciara                                          |  Zeichenkette        |
| 12.2341235211                                  |  Dezimalzahl             |
| true                                           |  BOOLEAN     |
| oben,unten                                     |  Aufzählungstyp         |
| .f},ÌúþÃ¸ìîìbõ©/=¹ryïòƒÇâ‘hðÂ.š¿ã‘q            |  Blob            |
| {name: "Meier", vorname: "Maxwell", alter: 21} |  RECORD      |

#### Aufgabe 2

Diskutieren Sie den Unterschied zwischen den folgenden Darstellungen von Verbunds-Typen "Noten". Halten sie ihre Erkenntnisse schriftlich fest.

**Darstellung 1**

Note:  
Tabelle  
| Wert     | Name |
|----------|------|
| 5.4      | Marcel Maier |

**Darstellung 2**

Note:  
Jason = Struktur  
{Wert = 5.4, Name = Marcel Maier}

#### Aufgabe 3

Finden sie die ASCII Codes für die folgenden Zeichen:

| Zeichen | Code dez | Code hex |
|---|---|---|
| + | 43 |2B |
| n | 110 | 6E |
| TAB | 9 | 09 |
| **CR** Zeilensprung | 13 | 0D |
| **LF** neue Zeile | 10 | 0A |
| **Leerzeichen** | 32 | 20 |
| **0** - 9 | 48 - 57 | 30 - 39 |
| **A** - Z | 65 - 90  | 41 - 5A |
| **a** - z | 97 - 122 | 61 - 7A |
| **DEL** | 127 | 7F |

## Datenstrukturen

<details> 
  <summary>Datensatz / Record / Tupel</summary>

* Es verfügt Werte, die in ander Werte enthalten sind - in fest definierten Anzahl und Folge
* besteht aus mehreren Elementen - Datenfeld
Beispiel: ID=12, Vorname=Hans, Nachname=Wenger, Telefonnummer=07911111111, Adresse=Zuercherstrasse 12
</details>

<details> 
  <summary>Array</summary>

* speichert mehrere Variabeln vom gleichen Datentyp
* jedes einzelnen Element hat die Möglichkeit zugriff über einen Index
* mehrdimensional (2D,3D, ...), z.B. Tabellen
Beispiel: [12, 45, 23, 38, 28], ["Hans", "Werner", "Sabine", "Rafael", "Susanne"]
</details>

<details> 
  <summary>VerketteteListe</summary>

* Liste von Elementen, die dynamisch wachsen
* Jedes Element zeigt auf das nächste Element
* die Elemente werden eins nach dem anderen verarbeitet
* einfach-verkettete-Liste nur von vorne nach hinten, doppelt-verkettete-Liste kann auch Rückwärts durchlauft werden
Beispiel: Am besten kannst du dir eine Liste vorstellen wie ein Fahrstuhl.
</details>

<details> 
  <summary>Stapelspeicher/ Stack</summary>

* die gespeicherten Objekte können nur in **umgekehrter Reihenfolge** wieder gelesen werden
* LIFO Prinzip, Last-In-First-Out
* Die funktion der zur letzt verarbeitet wurde wird zuerst abgearbeitet, evt. rückgabwert zurückgeben und dann wird gelöscht, dann wird die zuvoraufgerufte funktion verarbeitet
* Funktion verwalten und werte organisieren
* Stacks auch als einfach verkettete Liste/Dynamische Array verwirklichen
</details>

<details> 
  <summary>Warteschlange</summary>

* die gespeicherten Objekte können nur in den gleichen Reihenfolge wieder gelesen werden
* FIFO-Prinzip, First-In-First-Out:
Stell dir eine Perlenkette vor: Perlen kannst du nur an den Enden auffädeln oder entfernen, ohne die Kette zu zerstören. Genauso funktioniert eine Queue mit Datensätzen.
* wird meist als einfach verkettete Liste oder als dynamisches Feld realisiert
</details>

<details> 
  <summary>Vorrangwarteschlange</summary>

* Prioritätswarteschlange; wird die Elemente priorisiert
* sortiert das Objekt gemäss der gegebenen Proirität
</details>

<details> 
  <summary>Graph</summary>
Ein Graph besteht aus einer Menge an Knoten V und Knoten E
  
* enthält Referenzen auf mehrere Objekte
* kanten können gerichtet und ungerichtet sein
* den Kontengrad gibt an wie viele Kanten an einem Knoten hängen
* Ein Graph kann zusammenhängend sein; d.h gibt es Pfade zwischen allen Knoten.
* Gewichtete Graphen: zusätzliche Werte auf den Kanten, Entfernungen oder Kosten, nützlich für Berechnungen wie die kürzeste Route.
</details>

<details> 
  <summary>Baum</summary>

* Binärbaum: Ein Baum, bei dem jeder Knoten höchstens zwei Nachfolger hat – links und rechts.
* Tiefe: Die Anzahl der Kanten vom Knoten zur Wurzel.
* Höhe: Die maximale Tiefe aller Blätter im Baum.
* Größe: Die Gesamtzahl der Knoten im Baum.
* Vollständiger Binärbaum: Alle Ebenen sind vollständig gefüllt, außer der letzten, die von links nach rechts aufgefüllt ist.
* Partiell geordneter Baum: Knoten sind markiert und folgen einer Ordnung: Alle Knoten im linken Teilbaum sind kleiner oder gleich der Wurzel, im rechten Teilbaum größer oder gleich.
</details>

<details> 
  <summary>Heap</summary>

* Es vereint die Datnestruktur eines Baums mit dem Operationen einer Vorrangwarteschlange
* Speicherung von Mengen, unterstützt verschiedene Operationen: z.B. einfügen und entfernen der Elemente
* Flexible Größe bis zur Speichergrenze auf Prozessebene
* Durch schwierige interne Verwaltung, Anlegen und Entnehmen langsamer
* Ohne Garbage Collector manuelle Freigabe des Speichers
</details>

<details> 
  <summary>Hashtabelle</summary>

* eine spezielle Indexstruktur, bei der die Speicherposition direkt berechnet werden kann
* Informationen abspeichern

Beispiel:
Key: Paul
value: Telefon#

Hashfunktion  (key) -> Indexnummer
Hashfunktion  (Paul) -> 3
Hashfunktion  (Person) -> 1
Hashfunktion  (Person) -> 2
Hashfunktion  (Person) -> 4
Hashfunktion  (jemand) -> 3, die 3 ist vergeben, daraus wird ein link erstellt auch chaining gennant
</details>

--------

# Json - JavaScript Object Notation
TAG 4, 08.09.2025 

JASON ist ein Textformat um Daten zu speichern und Transportieren. 

ähnlich wie XML
APIs erstellen
leicht um hin und zurück zu senden, wegen den kleinen datei grösse
nicht viele open und closing tags, macht es leichter zu lesen und verstehen als XML
ist kompatibel mit mehrere Sprachen
wird mit JavaScript verarbeitet

**Typen**
Strings     "Hello World" "P"
Number      10  1.5 -30  1.2e350
Booleans    true false
null        steht für nichts
Arrays      "[]" unterteilt man mit einem Komma
Object      "{}"

**JASON Daten**
JASON Daten werden werden als Name-Wert Paar geschrieben: "firstName":"John"

**JASON Objekte**


**JASON Arrays**

### Wissenstreppe

-----------
# Normalisierung
Tag 6, 29.09.2025

### Relationale Datenbank (1-3NF)
**ACID-Model**  

**Vorteile von relationalen Datenbanken**  

**Begriffserklärung**  
<img width="860" height="300" alt="image" src="https://github.com/user-attachments/assets/2a9dd643-d42a-4b19-9f66-15166f9ed5a1" />








