---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben von Einstellungen zum Lesen aus der Projektdatenbank."
type: docs
weight: 75
url: /de/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Ermöglicht das Angeben von Einstellungen zum Lesen aus der Projektdatenbank.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Ruft die Verbindungszeichenfolge ab. |
| [getDriverClassName()](#getDriverClassName--) | Gibt einen Namen der JDBC-Treiberklasse zurück. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Setzt die Verbindungszeichenfolge. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Setzt einen Namen der JDBC-Treiberklasse. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Ruft die Verbindungszeichenfolge ab.

**Returns:**
java.lang.String - die Verbindungszeichenfolge.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Gibt einen Namen der JDBC-Treiberklasse zurück. Der Standardtreiberklassenname ist "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - Treiberklassenzeichenfolge.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Setzt die Verbindungszeichenfolge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Verbindungszeichenfolge. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Setzt einen Namen der JDBC-Treiberklasse. Der Standardtreiberklassenname ist "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Name der JDBC-Treiberklasse. |

