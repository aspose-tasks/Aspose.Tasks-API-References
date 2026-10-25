---
title: "Rsc.Work"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad total de tiempo programado para un recurso en una tarea"
type: docs
weight: 690
url: /es/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

La cantidad total de tiempo programado para un recurso en una tarea.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


