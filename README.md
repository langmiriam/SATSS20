# LaTeX kompilieren mit Glossar und Biber
Folgende Commands in der Reihenfolge ausführen:
1. pdflatex SATArbeit.tex
2. makeglossaries SATArbeit
3. biber SATArbeit
4. pdflatex SATArbeit.tex
Der Command makeglossaries benoetigt eventuell Perl. Das kann von http://strawberryperl.com/ heruntergeladen werden.

## Vereinfachung im TexMaker
Im Texmaker kann die Kompilierung selbst angegeben werden. 
- Hierfür auf "Benutzer/in" -> "Eigene Befehle" -> "Eigene Befehle editieren" klicken.
- Command benennen und folgendes als Command eintragen:
- pdflatex -synctex=1 -interaction=nonstopmode %.tex|makeglossaries %|biber %|pdflatex -synctex=1 -interaction=nonstopmode %.tex

## MikTex Update
Bei der Verwendung von MikTex unbedingt einmal die Console aufrufen und updaten, da unterschiedliche Versionen von "Biber" und "Bibtex" gerne zu Schwierigkeiten führen.
1. Strg + Esc und "MikTex" eingeben
2. MikTex Console aufrufen
3. In den Administrator Modus wechseln
4. "Updates" anklicken
5. "Check for updates" anklicken und warten
6. "Update Now" anklicken


