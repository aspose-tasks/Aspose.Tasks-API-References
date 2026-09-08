---
title: "Prj.NewTasksAreManual"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si las nuevas tareas se crean como manuales"
type: docs
weight: 550
url: /es/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Determina si las nuevas tareas se crean como manuales.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


