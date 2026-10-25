---
title: "Prj.MoveRemainingStartsForward"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si el inicio de las porciones restantes de tareas programadas para comenzar más tarde debe adelantarse a la fecha de estado"
type: docs
weight: 520
url: /es/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Determina si el comienzo de las porciones restantes de tareas programadas para haber comenzado más tarde debe adelantarse a la fecha de estado.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


