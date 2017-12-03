#####################################################
# GetDKP Plus
# Authors: Charla, Corgan, WalleniuM, Sylna
# $LastChangedDate: 2009-03-09 17:16:25 +0100 (Mo, 09 Mrz 2009) $
# $LastChangedBy: sylna $
#####################################################

SUPPORT FORUM: http://www.eqdkp-plus.com/e107_plugins/forum/forum_viewforum.php?11

---------------------

-> German <- 
Beschreibung:
===============

DKP Informationen ingame verf�gbar machen, ist jetzt kein Problem mehr.
Das Addon zeigt euch die DKP Punkte und alle Items aller Spieler in einem Fenster an, die in eurem EQDKP enthalten sind. Ihr k�nnt in diesem Fenster nach Klassen, Namen, Dropgruppen, R�stungsGruppen filtern sowie geziehlt nach einem oder mehreren Spielern suchen. Ihr k�nnt sowohl die DKP�s wie auch die Items der Spieler �ber die fenster in einem beliebigen chat ausgeben lassen. Es wird bei Items die im chat gelinkt sind ein tooltip angezeigt wo enthalten ist wer das Item schon besitzt und wer es noch braucht, nat�rlich werden dort auch die dkps mit angezeigt und alle Tooltiplisten k�nnen auch wieder in einem chat ausgegeben werden.

Dazu biete euch GetDKP auch ein Versteigerungsmodul "Bet and Win" an, mit dem ihr in verschiedenen vorgegebenen regeln eure Items versteigern k�nnt und direkt seht wer wieviel geboten hatt und wieviel DKP dieser noch hatt. Man kann dann auch noch direkt den Gewinner per Knopfdruck im Chat ausgeben.

Mit dem LIVEDKP k�nnt ihr nun im Raid einzelnen Spielern oder auch dem ganzen Raid DKP�s geben oder auch abziehen. 

Es gibt ein Konfigurationsmenu wo ihr alle einstellung vornehmen k�nnt.


Features:
- Unterst�tzt voll MultiDKP
- Unterst�tzt Umlaute wie (��� usw)
- Fl�stert jemand mit dem Addon an und bekommt sofort eure Punkte zur�ck !
- Zeigt alle Items an die im EQDKP eingetragen wurden.
- Bei Klick auf ein im Chat gelinktes Item �ffnet sich ein weiterer Tooltip. In diesem wird angezeigt, wer dieses Item schon f�r wieviele Punkte bekommen hat. 
  Bei Setitems wird au�erdem angezeigt wer dieses Item noch braucht.
  Diese Informationen k�nnen dann in den Raid/Gruppen/Gildenchat gepostet werden.
- Zeigt alle Items und deren DKP Preise die in eurem EQDKP eingetragen sind.
- Detailanzeige �ber Itempreise. Bei DKP System mit unterschiedlichen Itempreisen werden die Min/Max/AVG Preise angezeigt
- Wenn die Option gesetzt ist, werden nur Spieler im Raid angezeigt.
- Ausgehende Fl�sterer (z.B. Spieler oder Itemsuche) werden nicht mehr angezeigt
- Es werden auch Spieler im Tooltip angezeigt, die keine DKP Punkte haben, sich aber im Raid befinden.
- Fl�sterer nach Spieler oder Items sind jetzt im Kamp abgeschaltet und Lags zu verhindern.
- Die Anzahl der auszugebenen Spieler die noch Bedarf auf ein Item haben, oder die ein Item schon bestizen kann begrentzt werden.
- Ihr k�nnt w�hrend eines Raids DKP Punkte von Spielern �ndern.
- Minimap Icon zum �ffnen des Konfigurationsmenu oder des GetDKPList fenster

LiveDKP
===============
Mit diesen Funktionen bleibt ihr w�rend eines Raid immer auf dem aktuellen Stand.
Als normaler Spieler m�sst ihr nichts weiter konfigurieren.

Lootmaster bzw CT Raidtracker Lootmaster:
Wenn ihr w�rend eines Raid im Raidtracker auf edit Notes eines Items klickt k�nnt ihr dort die Punkte eintragen, die dem Spieler abgezogen werden sollen.
z.B. ein Spieler bekommt ein Item f�r 100 DKP. Dann tragt ihr in die Notes "100 DKP" ein. Wichtig dabei ist, das "DKP" gro� geschrieben wird.
Wenn ihr multiDKP mit mehreren Konten habt habt, dann muss die Note "100 DKP Kontoname" hei�en. kontoname ist der name den ihr im eqdkp dem jeweiligen konto gegeben habt.
Der Spieler der diese Eintr�ge im Raidtracker macht, MUSS ein A haben oder Raidleiter sein und zus�tzlich /dkp livedkp on aktiviert haben. (default = on)
Wenn die Note im Raidtracker eingetragen wurde, wird im Raidchat darauf hingewiesen. Bei allen Spielern die GetDKP 4.0.1 (oder h�her) installiert haben werden 
die Punkte jetzt automatisch abgezogen. Die Ver�nderungen an den Punkten werden solange gespeichert (auch beim umloggen und zwischen Sessions) bis die 
DKP Daten erneut von eurem EQDKP aktualisiert werden. 

Der Lootmaster (oder berechtigter Spieler) kann au�erdem gezielt einzelnen Spielern oder dem ganzen Raid Punkte abziehen bzw. hinzuf�gen.
Befehle dazu weiter unten.

F�r hilfe einfach /gdc help eingeben.

Installation
===============

Einfach runterladen und den Ordner Getdkp in euren xxx\World of Warcraft\Interface\AddOns\ ordner kopieren. 

Da WoW leider keinen direkten Zugriff auf Dateien im Internet oder Dateien auf der Festplatte erlaubt, muss man vor einem Raid die Punkte einmal abrufen. 
Dies funktioniert �ber die Datei DKP.EXE, die mit beiligt. In dieser m�sst ihr die Pfade zu WoW und zu eurem EQDKP richtig eintragen.

1. Entpackt die GetDKP.zip und kopiert den GetDkp Ordner in euren /Interface/Addon Ordner
2. Benutzt das Programm DKP.EXE (im GetDKPData-Ordner) um die DKP Informationen runterzuladen. Passt dazu den Path zu eurer getdkp.php und eurem WOW Ordner an.
3. Startet das Spiel

- nach dem ersten einloggen solltet ihr als erstes mal das Konfigurationsmen� �ffnen "/gdc" und dort eure einstellungen vornehmen. 
  Vor jedem Raid ist darauf zu achten das im Konfigurationsmen� immer das richtige Konto eingetragen ist. 
  Sollte ihr die beschreibung des kontos den Instanznamen gleichgesetzt haben so wird bei betreten der Instanz automatisch das konnto ge�ndert.
  
  
  
  
Fenster�ffnen :
===============
/gdc �ffnet das Konfigurationsmen�
/gdl �ffnet das GetDKPList Fenster
/gdb �ffnet das Versteigerungmodul Bet and Win




Befehle ingame:
===============
/gdc status									-> Zeigt die Konfiguration
/gdc info [chat/gilde/raid/gruppe] 			-> Gibt EQDKP Informationens im jeweiligen Channel aus.
/gdc help									-> Zeigt diese Tabelle
/gdc whisperdkp [on/off]					-> Schaltet die Fl�sterfunktion f�r DKP Punkte ab
/gdc whisperhide [on/off] 					-> Wenn aktiv, werden ausgehende Fl�sterer nicht mehr angezeigt, wenn z.B. jemand seine Punkte abfragt.
/gdc buyerslimit xx 						-> Beschr�nkt die Anzahl der angezeigten Spieler die ein Item schon besitzen. xx muss eine Zahl zwischen 1 und 40 sein. 0 = alle
/gdc needlimit xx 							-> Beschr�nkt die Anzahl der angezeigten Spieler die ein Item noch nicht besitzen. xx muss eine Zahl zwischen 1 und 40 sein. 0 = alle
/gdc reset  								-> Setzt alle GETDKP Variablen auf einen Defaultwert
/gdco [gilde/gruppe/chat/raid/offizer] 		-> setzt den Ausgabechat f�r den Befehl /dkp

LiveDKP
===============
/dkp+ [Spielername / Raid ] [DKP] [Kontoname]		-> F�gt dem Spieler (oder allen Spielern im Raid) xx Punkte hinzu
/dkp- [Spielername / Raid ] [DKP] [Kontoname]		-> Zieht dem Spieler (oder allen Spielern im Raid) xx Punkte ab


Beispiele: 
/dkp+ Corgan 100 DKP1 - Addiere 100 Punkte zu Corgans DKP Punkten auf dem Konto DKP1
/dkp- Corgan 100 DKP1 - Zieht 100 Punkte von Corgans DKP Punkten auf dem Konto DKP1 ab
/dkp+ Raid 100 DKP1 - Addiere 100 Punkte auf die Punkte aller Spieler im Raid f�r das Konto DKP1


Whisperbefehle:
===============

dkp	[kontoname]	-> DKP Punkte

Beispiel:
Der Spieler Corgan hat GetDKP installiert und ihr wollt von ihm erfahren wieviele Punkte ihr habt.
/w corgan dkp [kontoname]
============================================================================================
