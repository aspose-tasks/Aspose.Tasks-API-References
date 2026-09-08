---
title: "Prj.MoveCompletedEndsBack"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si el final de las porciones completadas de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe volver a la fecha de estado"
type: docs
weight: 490
url: /es/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Determina si el final de las porciones completadas de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe retroceder a la fecha de estado.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


