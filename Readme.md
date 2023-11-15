# Satzung des LSV Degerfeld e.V.

Dieses Repository dient als Ablage für die Satzung des LSV Degerfeld e.V. in verschiedenen Formaten. Insbesondere wird die Satzung in LaTeX gepflegt und in PDF umgewandelt.



## Mitmachen

Die Satzung ist ein lebendiges Dokument. Wenn du einen Fehler findest oder eine Änderung vorschlagen möchtest, kannst du das gerne tun. Dazu kannst du entweder einen Pull Request erstellen oder eine E-Mail an [vorstand@lsv-degerfeld.de] schreiben.

Wenn du einen Pull Request erstellst, achte bitte darauf, dass du die Änderungen in der LaTeX-Datei `Satzung.tex` vornimmst. Die anderen Dateien werden automatisch generiert und bei einem Merge verworfen.

Wenn du eine E-Mail schreibst, gib bitte an, welche Änderungen du vorschlägst und warum. Wenn du möchtest, kannst du auch eine geänderte Version der Satzung mitschicken. Wir werden dann prüfen, ob wir die Änderungen übernehmen können.


## Kompilieren

Die Satzung wird in LaTeX geschrieben und in PDF umgewandelt. Am einfachsten lässt sich die Satzung mit [TeX Live](https://www.tug.org/texlive/) in einem Docker-Container kompilieren. Dazu muss Docker installiert sein. Anschließend kann die Satzung mit folgendem Befehl kompiliert werden:

```bash
docker run --rm -w /data/ -v `pwd`:/data texlive/texlive latexmk -pdf -pdflatex="pdflatex -interaction=nonstopmode" Satzung.tex
```


## Lizenz

Die Satzung des LSV Degerfeld e.V. steht unter der [Creative Commons Namensnennung 4.0 International Lizenz](https://creativecommons.org/licenses/by/4.0/). Das bedeutet, dass du die Satzung kopieren, verändern und weitergeben darfst, solange du den Namen des LSV Degerfeld e.V. nennst. Eine kommerzielle Nutzung ist nicht gestattet.


