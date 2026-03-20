# TRIAS-Auskünfte erstellen
## API-Zugang
Für Dokumentation und Zugang zur Schnittstelle: https://www.opendata-oepnv.de/ht/de/organisation/verkehrsverbuende/vrr/openvrr/api

## Software für API-Zugang
Für die Nutzung der API empfehlen wir ein passendes Tool, z.B.:
- Postman:  https://www.postman.com/
- Insomnia: https://insomnia.rest/

Die Nutzung eines Browsers alleine reicht nicht aus, da POST-Anfragen für TRIAS benötigt werden.

## Request erzeugen
Der Request wird über eine POST-Anfrage erzeugt. Der Body wird im XML-Format an die API geliefert. 
Beispiele für den Body sind in den Files zu finden
Die API Unterstützt u.a. folgende Bodys:
- [LocationInformationRequest](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/TRIAS/LocationInformationRequest.md)
- [StopEventRequest](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/TRIAS/StopEventRequest.md)
- TripRequest
  - [Mit Koordinaten als Input](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/TRIAS/TripRequest_Geoposition.md)
  - [Mit DHIDs als Input](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/TRIAS/TripRequest.md)

Der Body wird über einen POST-Request an den Server https://openservice-test.vrr.de/opendataT/trias geschickt.
Ein Token ist nicht notwendig.

Als Header wird benötigt:
- Content-Type=text/xml

Der Server antwortet mit einer XML-Datei, die den TRIAS-Spezifikationen entspricht.

## Links und weitere Informationen
OpenData: https://www.opendata-oepnv.de/ht/de/organisation/verkehrsverbuende/vrr/openvrr/api \
Nutzungsvereinbarung API: https://www.opendata-oepnv.de/ht/de/standards/nutzungsvereinbarung-api \
TRIAS-API: https://openservice-test.vrr.de/opendataT/trias \
TRIAS-Dokumentation: https://www.vdv.de/ip-kom-oev.aspx# 
