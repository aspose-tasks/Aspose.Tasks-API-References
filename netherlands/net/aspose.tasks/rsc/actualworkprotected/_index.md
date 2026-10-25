---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De hoeveelheid werk waardoor het werkelijke werk beschermd is."
type: docs
weight: 80
url: /nl/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

De hoeveelheid werk waardoor feitelijk werk beschermd is.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualWorkProtected te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


