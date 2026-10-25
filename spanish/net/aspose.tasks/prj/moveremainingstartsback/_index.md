---
title: "Prj.MoveRemainingStartsBack"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si el inicio de las porciones restantes de tareas programadas para comenzar después de la fecha de estado pero iniciadas antes debe moverse de nuevo a la fecha de estado."
type: docs
weight: 510
url: /es/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Determina si el comienzo de las porciones restantes de tareas programadas para iniciar después de la fecha de estado, pero que comenzaron antes, debe devolverse a la fecha de estado.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


