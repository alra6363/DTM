## Qgis

1) Vergleich SPD/CDU stimmenstärkere Partei regelbasiert darstellen

Regel  Olaf
```
 "SPD" > "CDU"
 ```
 Regel Armin
 ```
 "SPD" < "CDU"
 ```

 2) Ebene"Alpha" ergänzen und auf Symbolebene 1 setzen
&nbsp;

 ![image](https://github.com/Tilidin/DTM/assets/134683773/88303c0c-2791-40fb-b339-3580019618cf)

3) Regel für Ebene "Alpha": über "Einfache Füllung" unter "Füllfarbe" -> "Datendefinierte Übersteuerung" -> "bearbeiten"
![image](https://github.com/Tilidin/DTM/assets/134683773/39fb3bc1-e3b7-4f21-a181-bd4ee861bc66)

Grundprinzip:
```
set_color_part('black','alpha', 126)
```

Statt einen festen Alpha Wert, wird dieser wertebasiert aus einem anderen Attribut für jede Bezugseinheit verrechnet:
```
set_color_part('black','alpha', scale_linear( "G", 100000, 200000,230,0))
```
