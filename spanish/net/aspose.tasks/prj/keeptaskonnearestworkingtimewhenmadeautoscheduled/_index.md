---
title: "Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si las tareas manuales deben mantenerse en el horario laboral más cercano cuando se convierten en programadas automáticamente."
type: docs
weight: 400
url: /es/net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

Determina si las tareas manuales deben mantenerse en el horario laboral más cercano cuando se convierten en programadas automáticamente.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


