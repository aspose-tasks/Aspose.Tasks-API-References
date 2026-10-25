---
title: "Rsc.Start"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De datum waarop een toegewezen resource gepland staat om te beginnen met werken aan een taak."
type: docs
weight: 640
url: /nl/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

De datum waarop een toegewezen resource gepland staat om aan een taak te beginnen.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Voorbeelden

Toont hoe de Rsc.Start eigenschap te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


