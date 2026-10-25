---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método PrimaveraBaseReader. Devuelve una lista de los identificadores únicos de los proyectos"
type: docs
weight: 20
url: /es/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Devuelve una lista de los identificadores únicos de los proyectos.

```csharp
public List<int> GetProjectUids()
```

### Valor devuelto

Lista de los identificadores únicos de los proyectos.

## Ejemplos

Muestra cómo importar un proyecto desde un archivo XML de Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Ver también

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


