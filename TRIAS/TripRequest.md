# Beschreibung der XML-Struktur: TripRequest.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Trias version="1.2" xmlns="http://www.vdv.de/trias"
       xmlns:siri="http://www.siri.org.uk/siri"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <ServiceRequest>
        <siri:RequestorRef>VRRTriasT</siri:RequestorRef>
        <RequestPayload>
            <TripRequest>
                <Origin>
                    <LocationRef>
                        <StopPlaceRef>de:05513:5613</StopPlaceRef>
                        <LocationName>
                            <Text>Gelsenkirchen Hbf</Text>
                        </LocationName>
                    </LocationRef>
                    <DepArrTime>2026-03-17T14:00:00</DepArrTime>
                </Origin>
                <Destination>
                    <LocationRef>
                        <StopPlaceRef>de:05513:5457</StopPlaceRef>
                        <LocationName>
                            <Text>Gelsenkirchen Erle Forsthaus</Text>
                        </LocationName>
                    </LocationRef>
                </Destination>
                <Params>
                </Params>
            </TripRequest>
        </RequestPayload>
    </ServiceRequest>
</Trias>
```

## Allgemeine Struktur
Dieses Dokument beschreibt eine TRIAS TripRequest-Anfrage. Sie dient der Abfrage einer Verbindung zwischen zwei Haltestellen.

## Elemente

### Trias
Root-Element mit Version 1.2 und den benötigten Namespaces.

### ServiceRequest
**RequestorRef**: Identifiziert den anfragenden Client (hier: VRRTriasT).

### TripRequest
Definiert die Verbindungsanfrage.

#### Origin
- **StopPlaceRef**: DHID der Start-Haltestelle (de:05513:5613 = Gelsenkirchen Hbf).
- **LocationName/Text**: Lesbarer Name der Start-Haltestelle.
- **DepArrTime**: Startzeit der Reise.

#### Destination
- **StopPlaceRef**: DHID der Ziel-Haltestelle (de:05513:5457 = Gelsenkirchen Erle Forsthaus).
- **LocationName/Text**: Lesbarer Name der Ziel-Haltestelle.

#### Params
Leeres Element für optionale Parameter.
