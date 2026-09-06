---
title: "MspDbSettings"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite establecer las opciones necesarias para leer datos del proyecto desde la base de datos de MS Project Server."
type: docs
weight: 161
url: /es/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Permite establecer las opciones necesarias para leer datos del proyecto desde la base de datos de MS Project Server.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Inicializa una nueva instancia de la clase [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Obtiene el GUID del proyecto a leer. |
| [getSchema()](#getSchema--) | Obtiene el esquema del MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Establece el esquema del MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Inicializa una nueva instancia de la clase [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionString | java.lang.String | la cadena de conexión especificada. |
| projectGuid | java.util.UUID | el GUID especificado de un proyecto a leer. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Obtiene el GUID del proyecto a leer.

**Returns:**
java.util.UUID - el GUID del proyecto a leer.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Obtiene el esquema del MS Project Server. El valor predeterminado es "pub".

**Returns:**
java.lang.String - el esquema del MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Establece el esquema del MS Project Server. El valor predeterminado es "pub".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el esquema del MS Project Server. |

