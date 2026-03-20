# RapidJSON-Requests erstellen
## API-Zugang
Für Dokumentation und Zugang zur Schnittstelle: https://www.opendata-oepnv.de/ht/de/organisation/verkehrsverbuende/vrr/openvrr/api

## Software für API-Zugang
Für die Nutzung der API empfehlen wir ein passendes Tool, z.B.:
- Postman:  https://www.postman.com/
- Insomnia: https://insomnia.rest/

Die Nutzung eines Browsers reicht für Anfragen aus, da GET-Requests erstellt werden.

## Request erzeugen
Der Request wird über eine GET-Anfrage erstellt.

Die API unterstützt u.a.:
- [Addinfo-Requests für Störungsmeldungen](https://github.com/BaserVRR/TRIAS-Beispiele/blob/main/rapidJSON/Addinfo-Request.md):\
  https://openservice-test.vrr.de/openservice/XML_ADDINFO_REQUEST?filterShowLineList=0&filterShowStopList=0&outputFormat=rapidJSON&filterProviderCode=ZTP-PROD

Die URL wird mit entsprechenden Parametern bestückt und abgeschickt.

Der Server antwortet mit einer rapidJSON Datei.
