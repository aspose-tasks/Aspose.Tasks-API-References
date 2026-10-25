---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de PrimaveraXerReader. Inicializa una nueva instancia de la clase PrimaveraXerReader"
type: docs
weight: 10
url: /es/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Inicializa una nueva instancia de la clase [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| xerFilePath | Cadena | Ruta al archivo .xer donde se encuentra el proyecto o los proyectos de Primavera. |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Inicializa una nueva instancia de la clase [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo con contenido XER de Primavera. |

### Ver también

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


