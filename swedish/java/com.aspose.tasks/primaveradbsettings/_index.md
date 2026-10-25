---
title: "PrimaveraDbSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ställa in nödvändiga alternativ för att läsa projektdata från Primavera-databasen."
type: docs
weight: 201
url: /sv/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

Tillåter att ställa in nödvändiga alternativ för att läsa projektdata från Primavera-databasen.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | Initierar en ny instans av klassen [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getProjectId()](#getProjectId--) | Hämtar id för projektet som ska läsas. |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


Initierar en ny instans av klassen [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connectionString | java.lang.String | den angivna anslutningssträngen. |
| projectId | int | det angivna id:t för ett projekt att läsa. |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


Hämtar id för projektet som ska läsas.

**Returns:**
int - id för projektet att läsa.
