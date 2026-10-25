---
title: "Clase PrimaveraXmlReader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.PrimaveraXmlReader. Representa un lector que permite recuperar los UID del proyecto desde un archivo XML de Primavera"
type: docs
weight: 1400
url: /es/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Representa un lector que permite recuperar los UID de proyecto de un archivo Primavera XML.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Inicializa una nueva instancia de la clase `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Inicializa una nueva instancia de la clase `PrimaveraXmlReader`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Devuelve una lista de los objetos de información breve del proyecto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Devuelve una lista de los identificadores únicos de los proyectos. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Carga el proyecto con el identificador único especificado. |

## Ejemplos

Muestra cómo examinar la información de proyectos cortos desde un archivo XML de Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Ver también

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


