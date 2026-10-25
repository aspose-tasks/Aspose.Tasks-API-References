---
title: "Rsc.RegularWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad total de trabajo sin horas extra programado para ser realizado por el recurso"
type: docs
weight: 570
url: /es/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

La cantidad total de trabajo sin horas extra programado para ser realizado por el recurso.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


