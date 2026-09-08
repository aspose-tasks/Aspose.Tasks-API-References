---
title: "SplitPartCollection.ToArray"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método SplitPartCollection. Copia todas las partes de la colección a una nueva matriz"
type: docs
weight: 40
url: /es/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Copia todas las partes de la colección a una nueva matriz.

```csharp
public SplitPart[] ToArray()
```

### Valor devuelto

Una matriz de objetos [`SplitPart`](../../splitpart/).

## Ejemplos

Muestra cómo trabajar con colecciones de partes divididas.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// iterar sobre partes divididas
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// obtener la parte por índice
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// realizar alguna operación con la primera parte dividida de la tarea
```

### Ver también

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


