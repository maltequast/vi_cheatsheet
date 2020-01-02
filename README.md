# vi_cheatsheet

## Overview of VI syntax
1. Different Modes
2. Move the cursor
3. Copy / Paste
4. Search / Replace
5. Insert
6. Delete
7. Undo
8. Advanced Mode

### 1. Different Modes

Es gibt unterschiedliche Modi in VI.
* Editing Mode 
* Overview Mode (ESC)
* Visual Block Mode

### 2. Move the cursor

Im Overview mode kann der Cursor durch die Pfeiltasten bewegt werden. Alternativ können ebenfalls die Tastenkürzel 
*h*,*j*,*k*,*l* benutzt werden.

Um schnell an den Anfang einer Datei zu gelangen nutzt im Overview Mode die Taste *gg*.
Um ans Ende der Datei zu gelangen drückt *G*.
Mitte der Datei *M*.

Command | Explanation
------------ | -------------
*gg* | Anfang einer Datei
*M* | Mitte einer Datei
*G* | Ende einer Datei

#### Bewegen innerhalb von Zeilen /Wortanfänge

Command | Explanation
------------ | -------------
*w* | nächste Wort
*W* | nächste Wort (TODO: punctuation)
*e* | Wortende
*E* | Wortende (TODO: punctuation)
*0* | Zeilenanfang
*$* | Zeilenende


## 3. Copy / Paste

Command | Explanation
------------ | -------------
*yy* | Kopieren
*p* | Einfügen
*5yy* | e.g. 5 Zeilen kopieren

## 6. Delete

Command | Explanation
------------ | -------------
*dd* | Zeile löschen
*dw* | bis zum nächsten Wort löschen
*de* | bis zum Ende des aktuellen Wortes löschen

## 7. Undo

Command | Explanation
------------ | -------------
*:u* | letzten Schritt rückgängig machen

## Save

Command | Explanation
------------ | -------------
*:wq* | Speichern und Verlassen
*:q!* | Verlassen OHNE speichern
*:saveas | speichern als
