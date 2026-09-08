---
title: "Clase SplitPartCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.SplitPartCollection clase. Colección que representa las porciones de una tarea"
type: docs
weight: 2300
url: /es/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Colección que representa las porciones de una tarea.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Obtiene el número de partes en la colección. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Recupera la parte dividida de una tarea en el índice dado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Copia todas las partes de la colección a una nueva matriz. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


