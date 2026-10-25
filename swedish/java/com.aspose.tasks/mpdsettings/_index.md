---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange nödvändiga alternativ för att läsa projektdata från MPD-formatet MS Access-databasfilformat."
type: docs
weight: 160
url: /sv/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

Tillåter att ställa in nödvändiga alternativ för att läsa projektdata från MPD-format (MS Access-databasfilformat).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | Initierar en ny instans av klassen `MpdSettings`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getProjectId()](#getProjectId--) | Returnerar id för projektet som ska läsas. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


Initierar en ny instans av klassen `MpdSettings`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connectionString | java.lang.String | den angivna anslutningssträngen. |
| projectId | int | det angivna id:t för ett projekt att läsa. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Returnerar id för projektet som ska läsas.

**Returns:**
int - id för projektet att läsa.
