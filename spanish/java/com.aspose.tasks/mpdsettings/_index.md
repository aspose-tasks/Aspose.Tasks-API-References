---
title: "MpdSettings"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite establecer las opciones necesarias para leer datos del proyecto desde el formato MPD de base de datos MS Access."
type: docs
weight: 160
url: /es/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

Permite establecer las opciones necesarias para leer datos del proyecto desde el formato MPD (formato de archivo de base de datos MS Access).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | Inicializa una nueva instancia de la clase `MpdSettings`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getProjectId()](#getProjectId--) | Devuelve el id del proyecto a leer. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


Inicializa una nueva instancia de la clase `MpdSettings`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionString | java.lang.String | la cadena de conexión especificada. |
| projectId | int | el id especificado de un proyecto a leer. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Devuelve el id del proyecto a leer.

**Returns:**
int - id del proyecto a leer.
