---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe om de benodigde opties in te stellen om projectgegevens te lezen uit MPD‑formaat MS Access‑databasabestand."
type: docs
weight: 160
url: /nl/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

Staat toe om de benodigde opties in te stellen om projectgegevens uit het MPD-formaat (MS Access-databasebestandformaat) te lezen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | Initialiseert een nieuw exemplaar van de `MpdSettings`‑klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getProjectId()](#getProjectId--) | Retourneert de id van het te lezen project. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


Initialiseert een nieuw exemplaar van de `MpdSettings`‑klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connectionString | java.lang.String | de opgegeven verbindingsreeks. |
| projectId | int | de opgegeven id van een project om te lezen. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Retourneert de id van het te lezen project.

**Returns:**
int - id van het project om te lezen.
