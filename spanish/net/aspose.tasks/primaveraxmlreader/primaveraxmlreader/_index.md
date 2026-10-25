---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor PrimaveraXmlReader. Inicializa una nueva instancia de la clase PrimaveraXmlReader"
type: docs
weight: 10
url: /es/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Inicializa una nueva instancia de la clase [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templatePath | Cadena | Ruta a la plantilla donde se encuentran los proyectos Primavera Xml |

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

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Inicializa una nueva instancia de la clase [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo que contiene el contenido de Primavera Xml. |

## Ejemplos

Muestra cómo importar un proyecto desde una secuencia Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### Ver también

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


