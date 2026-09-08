---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La cantidad de trabajo a través de la cual el trabajo extra real está protegido"
type: docs
weight: 60
url: /es/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

La cantidad de trabajo a través de la cual se protege el trabajo extra real.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


