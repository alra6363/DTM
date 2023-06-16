# Airbnb-Daten Berlin
## 1. Download der Daten
Benötigt sind die Datein review.csv neihbourhoods.geojson und listings.csv

![image](https://github.com/alra6363/DTM/assets/134683763/1d6ee6cc-5527-478b-845f-debb5d54e348)

Unter: http://insideairbnb.com/get-the-data

## 2. Import der Daten 
neighbourhoods.geojson als unterliegende Geometrie der Nachbarschaften sowie Import der listings

![image](https://github.com/alra6363/DTM/assets/134683763/5423c651-25d8-4e82-a986-3d6ae226823c)

## 3. Sortierung nach Nachbarschaften
duplizierung der listings -> entire dpt 
                             private room
                             shared  room
Abfrageerstellung 
room_type ) entire home
room_type = private room
room type = shared room
-> bei Rechtsklick und Filter

## 4. Durchschnittspreis der Airbnbs berechnen (shared rooms)
### Gitter erstellen
500m Seitenlänge -> Kurze Diagonale 866,025m

### nach Position Selektieren
Gitter in Berlin
### Attribute nach Position verknüpfen (Zusammenfassung)
![image](https://github.com/alra6363/DTM/assets/134683763/d3dfcd61-b8c6-45f0-be54-ec5d73d07f15)
Zusammenzufassende Felder: price
Zu berechende Zusammenfassungen: Durchschnitt
-> Klassifizierung nach Jenks

![image](https://github.com/alra6363/DTM/assets/134683763/796a200f-cbe3-4825-bf16-6161498bde0d)

## 5. Heatmap erstellen 
![image](https://github.com/alra6363/DTM/assets/134683763/9bb8393c-1707-43c5-9c46-b2f908631228)

### Hintergrund schwarz:
Projekt -> Eigenschaften -> Allgemein -> Hintergrundfarbe 

![image](https://github.com/alra6363/DTM/assets/134683763/c4007d8d-de09-43c6-9895-59a65cc00530)

### Auf andere Layer übertragen 
Rechtsklick auf Layer -> Stile -> Stil kopieren -> Rechtsklick andere Layer -> Stil einfügen

## 6. Drucklayout
airbnb logo unter : https://de.cleanpng.com/png-g1vjlg/
