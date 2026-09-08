---
title: "Rsc.Finish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De datum waarop een resource gepland staat om werk op alle toegewezen taken te voltooien"
type: docs
weight: 290
url: /nl/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

De datum waarop een resource gepland staat om werk op alle toegewezen taken te voltooien.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Finish gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


