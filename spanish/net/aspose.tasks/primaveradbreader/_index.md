---
title: "Clase PrimaveraDbReader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.PrimaveraDbReader. Representa un lector para leer información del proyecto desde Primavera DB."
type: docs
weight: 1350
url: /es/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Representa un lector para leer la información del proyecto desde la base de datos Primavera.

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Inicializa una nueva instancia de la clase [`PrimaveraXerReader`](../primaveraxerreader/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Devuelve una lista de los objetos de información breve del proyecto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Devuelve una lista de los identificadores únicos de los proyectos. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Carga el proyecto con el identificador único especificado. |

## Ejemplos

Muestra cómo obtener información breve de los proyectos desde una base de datos Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Ver también

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


