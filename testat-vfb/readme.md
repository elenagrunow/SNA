# Datensatz VfB-Netzwerk

## Inhalt
*Edges.csv (Edgelist)
*Nodes.csv (Nodelist)
*Codebuch.rm (Codierung der Datensätze)

## Ursprung und Datenerhebung 
Das Netzwerk ist ein ungerichtetes und ungewichtetes two-mode Akteursnetzwerk (Mitgliedschaft in Organisationen). Zur Unterscheidung zwischen Organisationen und Personen wird das Attribut type in der Nodelist erhoben.
Die Mitgliedschaft kann dabei eine klassische Mitgliedschaft in einem Verein sein, aber auch ein Beschäftigungsverhältnis.
Der Erhebungszeitraum besteht bis einschließlich zum 13. Februar 2021.
Die Daten wurden mithilfe der Auflistung auf der Website des VfB erhoben (https://www.vfb.de/de/1893/club/vfb-ag/organe-der-vfb-ag/).

# EDGE-Attribute

**id**
(eindeutige Codierung des Knoten)
Jede ID entspricht dem Namen einer Organisation oder einer Person, die unmittelbar mit dem VfB oder anderen Pateien, Verbänden usw. in Verbindung steht. 

**to**
(alle aktiven Mitgliedschaften der Person, soweit in dem Dokument recherchierbar, dazu gehört z.B. politische Partei, Unternehmen, Verbände, Vereine und weitere Organisationen)

**active**
1 = aktive Mitgliedschaft,
2 = inaktive Mitgliedschaft

# NODE-Attribute

**id**
Identische ID wie in der Edgelist zur Identifikation der Knoten. 

**type**
1 = Person,
2 = Organisation, Regierung, Unternehmen, Verband

**age**
Alter der involvierten Person:
1 = bis 25 Jahre,
2 = 30 bis 40 Jahre,
3 = 41 bis 60 Jahre,
4 = 61 und älter

**role**
1 = Vorstand,
2 = Aufsichtsrat,
3 = Unternehmen mit Kontakten zum Aufsichtsrat und zum Vorstand,
4 = Unternehmen mit Kontakten zum Vorstand,
5 = Unternehmen mit Kontakten zum Aufsichtsrat,

**representation**
(bezieht sich auf die Funktion innerhalb der VfB Gremien)
1 = Wirtschaft,
2 = Finanzen,
3 = Marketing,
4 = Sport,
5 = Kommunikation,
6 = Wissenschaft


**position**
Position im Unternehmen, der Organisation bei VfB
1 = Vorsitz,
2 = Stellvertreter,
3 = Mitglied in der VfB Organisation


**source**
Der Link der Quelle der Beziehung wird angegeben.
