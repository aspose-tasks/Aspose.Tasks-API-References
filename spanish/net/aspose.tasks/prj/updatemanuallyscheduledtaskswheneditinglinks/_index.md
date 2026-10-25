---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si las tareas manuales deben actualizarse cuando se editan los enlaces"
type: docs
weight: 770
url: /es/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

Determina si las tareas manuales deben actualizarse cuando los enlaces fueron editados.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.UpdateManuallyScheduledTasksWhenEditingLinks.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


