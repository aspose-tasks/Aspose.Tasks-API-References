---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Festlegen notwendiger Optionen zum Lesen von Projektdaten aus einer MS Project Server‑Datenbank."
type: docs
weight: 161
url: /de/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Ermöglicht das Festlegen notwendiger Optionen zum Lesen von Projektdaten aus einer MS Project Server‑Datenbank.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Initialisiert eine neue Instanz der [MspDbSettings](../../com.aspose.tasks/mspdbsettings)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Ermittelt die GUID des zu lesenden Projekts. |
| [getSchema()](#getSchema--) | Ermittelt das Schema des MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Legt das Schema des MS Project Server fest. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Initialisiert eine neue Instanz der [MspDbSettings](../../com.aspose.tasks/mspdbsettings)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connectionString | java.lang.String | die angegebene Verbindungszeichenfolge. |
| projectGuid | java.util.UUID | die angegebene guid eines Projekts zum Lesen. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Ermittelt die GUID des zu lesenden Projekts.

**Returns:**
java.util.UUID - die guid des Projekts zum Lesen.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Liest das Schema des MS Project Server. Der Standardwert ist "pub".

**Returns:**
java.lang.String - das Schema des MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Legt das Schema des MS Project Server fest. Der Standardwert ist "pub".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | das Schema des MS Project Server. |

