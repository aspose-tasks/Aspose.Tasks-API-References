---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe instellingen op te geven om te lezen uit de projectdatabase."
type: docs
weight: 75
url: /nl/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Staat toe instellingen op te geven om te lezen uit de projectdatabase.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Haalt de connection string op. |
| [getDriverClassName()](#getDriverClassName--) | Retourneert een naam van de JDBC driver class. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Stelt de connection string in. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Stelt een naam van de JDBC driver class in. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Haalt de connection string op.

**Returns:**
java.lang.String - de connection string.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Retourneert een naam van de JDBC driver class. De standaard driver class-naam is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - driver class string.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Stelt de connection string in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de connection string. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Stelt een naam van de JDBC driver class in. De standaard driver class-naam is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een naam van de JDBC driver class. |

