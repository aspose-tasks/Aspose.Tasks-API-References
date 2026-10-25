---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe om de benodigde opties in te stellen om projectgegevens uit de MS Project Server-database te lezen."
type: docs
weight: 161
url: /nl/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Staat toe om de benodigde opties in te stellen om projectgegevens uit de MS Project Server-database te lezen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Initialiseert een nieuw exemplaar van de klasse [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Haalt de GUID van het project op om te lezen. |
| [getSchema()](#getSchema--) | Haalt het schema van de MS Project Server op. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Stelt het schema van de MS Project Server in. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Initialiseert een nieuw exemplaar van de klasse [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connectionString | java.lang.String | de opgegeven verbindingsreeks. |
| projectGuid | java.util.UUID | de opgegeven GUID van een project om te lezen. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Haalt de GUID van het project op om te lezen.

**Returns:**
java.util.UUID - de GUID van het project om te lezen.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Haalt het schema van de MS Project Server op. De standaardwaarde is "pub".

**Returns:**
java.lang.String - het schema van de MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Stelt het schema van de MS Project Server in. De standaardwaarde is "pub".

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het schema van de MS Project Server. |

