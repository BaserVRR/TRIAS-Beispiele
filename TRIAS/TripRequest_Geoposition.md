
# Beschreibung der XML-Struktur: TripRequest_GeoPosition.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Trias version="1.1" xmlns="http://www.vdv.de/trias" xmlns:siri="http://www.siri.org.uk/siri" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"> 
    <ServiceRequest>
        <siri:RequestorRef>VRRTriasT</siri:RequestorRef>
        <RequestPayload>
            <TripRequest>
                <Origin>
                    <LocationRef>
                        <GeoPosition>
                            <Longitude>6.793499</Longitude>
                            <Latitude>51.219411</Latitude>
                        </GeoPosition>
                    </LocationRef>
                    <DepArrTime>2026-06-31T08:39:10</DepArrTime>
                </Origin>
                <Destination>
                    <LocationRef>
                        <GeoPosition>
                            <Longitude>6.793499</Longitude>
                            <Latitude>50.219411</Latitude>
                        </GeoPosition>
                    </LocationRef>
                </Destination>
                <Params>
                    <NumberOfResults>1</NumberOfResults>
                    <IncludeTrackSections>false</IncludeTrackSections>
                    <IncludeLegProjection>true</IncludeLegProjection>
                    <IncludeIntermediateStops>false</IncludeIntermediateStops>
                </Params>
            </TripRequest>
        </RequestPayload>
    </ServiceRequest>
</Trias>
```

## Allgemeine Struktur
Dieses Dokument beschreibt eine TRIAS **TripRequest**-Anfrage, bei der Start- und Zielort über **Geokoordinaten** definiert werden.

## Elemente

### Trias
Root-Element der TRIAS-Struktur, Version 1.1.

### ServiceRequest
- **RequestorRef**: Identifiziert den anfragenden Client (hier: VRRTriasT).

### TripRequest
Enthält die Routenanfrage.

#### Origin (Startpunkt)
- **GeoPosition**: Startkoordinaten.
  - *Longitude*: 6.793499
  - *Latitude*: 51.219411
- **DepArrTime**: Zeitpunkt des Reisebeginns (2026-06-31T08:39:10). Hinweis: Der 31. Juni ist im realen Kalender nicht existent.

#### Destination (Zielpunkt)
- **GeoPosition**: Zielkoordinaten.
  - *Longitude*: 6.793499
  - *Latitude*: 50.219411

#### Params
Parameter zur Steuerung der Ausgabe:
- **NumberOfResults**: 1 Ergebnis.
- **IncludeTrackSections**: false → Streckenabschnitte nicht einbeziehen.
- **IncludeLegProjection**: true → Geometrie/Projektionen der Fahrtabschnitte einbeziehen.
- **IncludeIntermediateStops**: false → Keine Zwischenhalte anzeigen.
