# Datensatz 25 reichste Youtuber

Codebuch Stand 2022-01 erstellt von Florian Striegl, Julia Dusemond, Lina Quotschalla, Pascal Eichner und Jessica Schreiner  

Inhalt

Edges_youtuber.csv (Edgelist)
Nodes_youtuber.csv (Nodelist)
Codebuch_youtuber.md (Codierung der Datensätze)

## Ursprung und Datenerhebung

Wir haben den Datensatz aus dem Vermögenmagazin der reichsten Youtuber sowie der Socialblade- Liste der Top 100 Youtube-Channels Deutschlands erhoben. Für unser Projekt analysieren wir die Top 25, deren Verbindungen und Einkommensquellen (aus welchen Bereichen auch außerhalb von Youtube z.B. Musik). Wir beziehen uns auf den Stand Februar 2022. 

Das Netzwerk ist ein ungerichtetes two-mode Akteursnetzwerk.

## EDGE-Attribute

**from**  
id des Youtubers/der Einnahmequelle(n), in zwei Buchstaben z.B. Simon Wiefels: sw

**to**  
type, Youtuber (0), Einkommensquellen als konkreter Name, z.B. Name des Podcasts, Buch, etc. (1)

**relation**  
1 = Zusammenarbeit (Erscheinen zusammen in mind. 1 Video), 3 = Welche Einnahmequellen hat die:der Youtuber:in? 


## NODE-Attribute

"99" steht für "keine Angabe"

**id**  
Identische ID wie aus der edgelist zur Identifikation der Knoten.

**person**  
Ganzer Name zusammengeschrieben z.B. SimonWiefels

**name**  
Name des Youtubekanals/der Einnahmequelle

**type**  
0 = youtuber:in, 1 = Einnahmequellen als konkreter Name (Bereiche wie z.B. Musik, Bücher, ...)

**youtubeabos**  
Anzahl der Abonnenten auf Youtube in ganzen Zahlen.

**Instagramfollower**  
Instagramfollower in ganzen Zahlen.

**TikTokFollower**  
Follower auf TikTok in ganzen Zahlen.

**Facebookfollower**  
Follower auf Facebook in ganzen Zahlen.

**wealth**  
Vermögen in ganzen Zahlen.

**salary**  
Einkommen pro Monat auf Youtube als Zahl. Z.B. 3000000 für drei Millionen.

**city**  
In welcher Stadt lebt der:die Youtuber:in, Stadtname

**birth**  
Jahrgang des Youtubers.

99 = für type 1, nicht def. Alter

**sex**  
Geschlecht des Youtubers
1 = male, 2 = female, 3 = divers

**country**   
Landname, in dem Youtuber lebt.

**management**  
Name des Managements, bei dem der/die Youtuber:in ist.

**category**  
Kategorie der Einnahmequelle, z.B. Podcast, Musik, Buch, ...
