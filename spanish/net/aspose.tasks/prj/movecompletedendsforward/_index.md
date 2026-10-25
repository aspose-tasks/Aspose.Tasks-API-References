---
title: "Prj.MoveCompletedEndsForward"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si el final de las partes completadas de tareas programadas para haber sido completadas antes de la fecha de estado pero iniciadas después debe moverse a la fecha de estado"
type: docs
weight: 500
url: /es/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Determina si el final de las porciones completadas de tareas programadas para haber finalizado antes de la fecha de estado pero que comenzaron después debe adelantarse a la fecha de estado.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


