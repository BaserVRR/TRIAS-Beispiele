# TRIAS-Auskünfte erstellen
Für Dokumentation und Zugang zur Schnittstelle: https://www.opendata-oepnv.de/ht/de/organisation/verkehrsverbuende/vrr/openvrr/api

## Software für API-Zugang
Für den Zugang zur API empfehlen wir ein passendes Tool, z.B.:
- Postman:  https://www.postman.com/
- Insomnia: https://insomnia.rest/

Die Nutzung eines Browsers alleine reicht nicht aus, da POST-Anfragen für TRIAS benötigt werden.

## Request erzeugen
Der Request wird über eine POST-Anfrage erzeugt. Der Body wird im XML-Format an die API geliefert. 
Beispiele für den Body sind in den Files zu finden
Die API Unterstützt u.a. 
- [LocationInformationRequest](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/LocationInformationRequest)
- [StopEventRequest](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/StopEventRequest)
- [TripAdressInput](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/Trip%20addressInput%20(Koordinaten))
- [TripRequest](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/TripRequest)

Der Body wird über einen POST-Request an den Server https://openservice-test.vrr.de/opendataT/trias geschickt.
Ein Token ist nicht notwendig.

Als Header wird benötigt:
- Content-Type=text/xml

Der Server antwortet mit einer XML-Datei, die den TRIAS-Spezifikationen entspricht.

