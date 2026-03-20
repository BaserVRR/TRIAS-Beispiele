
# Beschreibung der XML-Struktur: LocationInformationRequest.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Trias xmlns:siri="http://www.siri.org.uk/siri" xmlns="http://www.vdv.de/trias" xmlns:ns3="http://www.ifopt.org.uk/acsb" xmlns:ns4="http://www.ifopt.org.uk/ifopt" xmlns:ns5="http://datex2.eu/schema/1_0/1_0" version="1.2"> 
    <ServiceRequest>
        <siri:RequestTimestamp>2026-07-31T12:00:00+01:00</siri:RequestTimestamp>
        <Language>deu</Language>
        <RequestPayload>
            <LocationInformationRequest>
                <InitialInput>
                    <LocationName>Essen Hbf</LocationName>
                </InitialInput>
            </LocationInformationRequest>
        </RequestPayload>
    </ServiceRequest>
</Trias>
```

## Allgemeine Struktur
Dieses Dokument beschreibt eine TRIAS **LocationInformationRequest**-Anfrage. Sie dient der Abfrage von Orts- bzw. Haltestelleninformationen basierend auf einem eingegebenen Namen.

## Elemente

### Trias
Root-Element mit Version 1.2 und mehreren Namespaces (TRIAS, SIRI, IFOPT, DATEX II).

### ServiceRequest
- **RequestTimestamp**: Zeitpunkt der Anfrage.
- **Language**: Sprachangabe (hier: *deu* für Deutsch).

### RequestPayload / LocationInformationRequest
Dieser Block beschreibt die eigentliche Anfrage nach Standortinformationen.

#### InitialInput
- **LocationName**: Der eingegebene Suchbegriff. In diesem Fall wird nach **Essen Hbf** gesucht.

