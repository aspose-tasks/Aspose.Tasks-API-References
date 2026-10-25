---
title: "Rsc.RemainingWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El tiempo aún necesario para completar una tarea o conjunto de tareas"
type: docs
weight: 610
url: /es/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

El tiempo aún necesario para completar una tarea o conjunto de tareas.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


