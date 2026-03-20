
# Beschreibung der XML-Struktur: StopEventRequest.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Trias version="1.1" xmlns="http://www.vdv.de/trias"
       xmlns:siri="http://www.siri.org.uk/siri"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <ServiceRequest>
    <siri:RequestorRef>VRRTriasT</siri:RequestorRef>
    <RequestPayload>
      <StopEventRequest>
        <Location>
          <LocationRef>
            <StopPlaceRef>de:05513:5613</StopPlaceRef>
            <LocationName>
              <Text>Gelsenkirchen Hbf</Text>
            </LocationName>
          </LocationRef>
          <DepArrTime>2026-03-14T14:50:00Z</DepArrTime>
        </Location>
        <Params>
          <StopEventType>departure</StopEventType>
          <NumberOfResults>5</NumberOfResults>
          <IncludeRealtimeData>true</IncludeRealtimeData>
        </Params>
      </StopEventRequest>
    </RequestPayload>
  </ServiceRequest>
</Trias>
```

## Allgemeine Struktur
Dieses Dokument beschreibt eine TRIAS StopEventRequest-Anfrage. TRIAS ist ein standardisiertes Austauschformat für Fahrplan- und Echtzeitdaten im öffentlichen Verkehr.

## Elemente

### Trias
Wurzelelement mit Versionsangabe und Namespace-Definitionen.

### ServiceRequest
**RequestorRef**: Identifiziert den anfragenden Client (hier: VRRTriasT).

### RequestPayload / StopEventRequest
Enthält die Abfrage nach Abfahrts- oder Ankunftsereignissen.

#### Location
- **StopPlaceRef**: DHID der Haltestelle (de:05513:5613 für Gelsenkirchen Hbf).
- **LocationName/Text**: Lesbarer Haltestellenname.
- **DepArrTime**: Zeitpunkt der Abfrage in UTC.

#### Params
- **StopEventType**: Art des Ereignisses (departure = Abfahrten).
- **NumberOfResults**: Anzahl gewünschter Ergebnisse.
- **IncludeRealtimeData**: Echtzeitinformationen einbeziehen.
