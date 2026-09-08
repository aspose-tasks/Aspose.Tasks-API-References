---
title: "Rsc.ActualOvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad real de trabajo extra ya realizado por el recurso asignado a tareas"
type: docs
weight: 50
url: /es/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

La cantidad real de trabajo extra ya realizado por el recurso asignado a las tareas.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


