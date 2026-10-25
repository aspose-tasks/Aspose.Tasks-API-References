---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Festlegen notwendiger Optionen zum Lesen von Projektdaten aus dem MPD‑Format der MS‑Access‑Datenbankdatei."
type: docs
weight: 160
url: /de/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

Ermöglicht das Festlegen notwendiger Optionen zum Lesen von Projektdaten aus dem MPD-Format (MS Access-Datenbankdateiformat).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | Initialisiert eine neue Instanz der `MpdSettings`‑Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getProjectId()](#getProjectId--) | Gibt die ID des zu lesenden Projekts zurück. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


Initialisiert eine neue Instanz der `MpdSettings`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connectionString | java.lang.String | die angegebene Verbindungszeichenfolge. |
| projectId | int | die angegebene ID eines zu lesenden Projekts. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Gibt die ID des zu lesenden Projekts zurück.

**Returns:**
int - ID des zu lesenden Projekts.
