---
title: "Rsc.RemainingOvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad de tiempo extra programado restante"
type: docs
weight: 600
url: /es/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

La cantidad de horas extra programadas restantes.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


