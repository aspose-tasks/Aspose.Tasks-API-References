---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si los nuevos recursos o tareas se añaden automáticamente a un grupo de recursos o tareas"
type: docs
weight: 50
url: /es/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Determina si los nuevos recursos o tareas se añaden automáticamente a un grupo de recursos o tareas.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.AutoAddNewResourcesAndTasks.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


