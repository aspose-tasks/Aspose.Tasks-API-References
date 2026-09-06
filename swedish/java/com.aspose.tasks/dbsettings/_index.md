---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange inställningar för att läsa från projektdatabasen."
type: docs
weight: 75
url: /sv/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Tillåter att ange inställningar för att läsa från projektdatabasen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Hämtar anslutningssträngen. |
| [getDriverClassName()](#getDriverClassName--) | Returnerar ett namn på JDBC-drivrutinsklass. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Ställer in anslutningssträngen. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Ställer in ett namn på JDBC-drivrutinsklass. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Hämtar anslutningssträngen.

**Returns:**
java.lang.String - anslutningssträngen.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Returnerar ett namn på JDBC-drivrutinsklassen. Standarddrivrutinsklassnamnet är "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - drivrutinsklasssträng.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Ställer in anslutningssträngen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | anslutningssträngen. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Ställer in ett namn på JDBC-drivrutinsklassen. Standarddrivrutinsklassnamnet är "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett namn på JDBC-drivrutinsklassen. |

