---
title: "Rsc.ActualWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La cantidad de trabajo que ya ha sido realizado por el recurso asignado a tareas"
type: docs
weight: 70
url: /es/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

La cantidad de trabajo que ya ha sido realizado por el recurso asignado a las tareas.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


