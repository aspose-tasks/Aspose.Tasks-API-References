---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare le impostazioni per la lettura dal database del progetto."
type: docs
weight: 75
url: /it/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Consente di specificare le impostazioni per la lettura dal database del progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Ottiene la stringa di connessione. |
| [getDriverClassName()](#getDriverClassName--) | Restituisce il nome della classe driver JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Imposta la stringa di connessione. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Imposta il nome della classe driver JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Ottiene la stringa di connessione.

**Returns:**
java.lang.String - la stringa di connessione.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Restituisce il nome della classe driver JDBC. Il nome predefinito della classe driver è "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - stringa della classe driver.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Imposta la stringa di connessione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la stringa di connessione. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Imposta il nome della classe driver JDBC. Il nome predefinito della classe driver è "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un nome della classe driver JDBC. |

