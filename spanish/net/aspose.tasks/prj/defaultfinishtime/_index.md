---
title: "Prj.DefaultFinishTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El tiempo de finalización predeterminado de las tareas nuevas"
type: docs
weight: 230
url: /es/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

La hora de finalización predeterminada de las tareas nuevas.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


