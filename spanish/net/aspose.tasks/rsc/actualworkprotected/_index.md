---
title: "Rsc.ActualWorkProtected"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad de trabajo a través de la cual el trabajo real está protegido"
type: docs
weight: 80
url: /es/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

La cantidad de trabajo a través de la cual se protege el trabajo real.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


