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
*CTRL* + *d* or *u* | jump to the end of the screen

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

## 4. Search

Command | Explanation
------------ | -------------
*/searchterm* | Suchbegriff  - Vorwärtssuche GLOBAL mit *n* und  zurück mit *N* 
*?searchterm* | Suchbegriff - Rückwärtssuche GLOBAL
*:%s/searchterm/replaceterm/* | Suchen und ersetzen GLOBAL
*:s/searchterm/replaceterm/* | Replace in CURRENT row (all) occurences

### Outside of VI

Command | Explanation
------------ | -------------
*vi +/searchTermHere fileName* | Öffnen in VI und zum ersten Suchbegriff
*vim +LineNumber fileName* | Öffnen des Files und zu Zeile springen
*vi +commandHere fileName* | Kommand außerhalb von VI durchführen

## 5. Insert

Command | Explanation
------------ | -------------
*i* | insert here
*a* | insert append
*o* | open new line after this

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
