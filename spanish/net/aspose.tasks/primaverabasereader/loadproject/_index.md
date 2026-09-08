---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método PrimaveraBaseReader. Carga el proyecto con el identificador único especificado"
type: docs
weight: 30
url: /es/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Carga el proyecto con el identificador único especificado.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectUid | Int32 | Identificador único del proyecto a cargar. |

### Valor devuelto

Proyecto con el identificador único especificado del archivo multiproyecto especificado. Nulo si el proyecto no existe.

## Ejemplos

Muestra cómo cargar un proyecto desde un archivo XML de Primavera cuando se conoce el uid del proyecto.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


