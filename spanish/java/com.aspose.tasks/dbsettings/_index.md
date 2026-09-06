---
title: "DbSettings"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar configuraciones para leer de la base de datos del proyecto."
type: docs
weight: 75
url: /es/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Permite especificar configuraciones para leer de la base de datos del proyecto.
## Métodos

| Método | Descripción |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Obtiene la cadena de conexión. |
| [getDriverClassName()](#getDriverClassName--) | Devuelve un nombre de clase de controlador JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Establece la cadena de conexión. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Establece un nombre de clase de controlador JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Obtiene la cadena de conexión.

**Returns:**
java.lang.String - la cadena de conexión.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Devuelve un nombre de clase de controlador JDBC. El nombre de clase de controlador predeterminado es "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - cadena de clase de controlador.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Establece la cadena de conexión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la cadena de conexión. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Establece un nombre de clase de controlador JDBC. El nombre de clase de controlador predeterminado es "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un nombre de clase de controlador JDBC. |

