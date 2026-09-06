---
title: "PrimaveraDbReader"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un lector para leer la información del proyecto de la base de datos de Primavera"
type: docs
weight: 200
url: /es/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Representa un lector para leer la información del proyecto de la base de datos de Primavera
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Inicializa una nueva instancia de la clase [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Métodos

| Método | Descripción |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Carga el proyecto con el identificador único especificado. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Inicializa una nueva instancia de la clase [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Configuraciones que especifican cómo conectarse a la base de datos Primavera. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Carga el proyecto con el identificador único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectUid | int | Identificador único del proyecto a cargar. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
