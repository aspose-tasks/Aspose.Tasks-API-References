---
title: "SplitPartCollection.Item"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "SplitPartCollection property. Recupera una parte dividida de la tarea en el índice dado"
type: docs
weight: 20
url: /es/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Recupera la parte dividida de una tarea en el índice dado.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice de la parte. |

### Valor devuelto

una parte dividida.

## Observaciones

El índice comienza en cero. Devuelve null si el índice está fuera de los límites del arreglo.

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


