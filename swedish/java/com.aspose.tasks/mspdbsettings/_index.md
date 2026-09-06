---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ställa in nödvändiga alternativ för att läsa projektdata från MS Project Server-databas."
type: docs
weight: 161
url: /sv/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Tillåter att ställa in nödvändiga alternativ för att läsa projektdata från MS Project Server-databas.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Initierar en ny instans av klassen [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Hämtar guid för projektet som ska läsas. |
| [getSchema()](#getSchema--) | Hämtar schemat för MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Ställer in schemat för MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Initierar en ny instans av klassen [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connectionString | java.lang.String | den angivna anslutningssträngen. |
| projectGuid | java.util.UUID | den angivna guid för ett projekt att läsa. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Hämtar guid för projektet som ska läsas.

**Returns:**
java.util.UUID - guid för projektet att läsa.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Hämtar schemat för MS Project Server. Standardvärdet är "pub".

**Returns:**
java.lang.String - schemat för MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Ställer in schemat för MS Project Server. Standardvärdet är "pub".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | schemat för MS Project Server. |

