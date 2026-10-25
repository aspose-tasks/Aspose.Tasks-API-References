---
title: "Clase PrimaveraXerReader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.PrimaveraXerReader. Representa un lector para leer los UID del proyecto desde un archivo Primavera XER."
type: docs
weight: 1390
url: /es/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Representa un lector para leer los UID de proyecto de un archivo Primavera XER.

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Inicializa una nueva instancia de la clase `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Inicializa una nueva instancia de la clase `PrimaveraXerReader`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Devuelve una lista de los objetos de información breve del proyecto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Devuelve una lista de los identificadores únicos de los proyectos. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Carga el proyecto con el identificador único especificado. |

## Ejemplos

Muestra cómo examinar la información de proyectos cortos desde un archivo Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Ver también

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


