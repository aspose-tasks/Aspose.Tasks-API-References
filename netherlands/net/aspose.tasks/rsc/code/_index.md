---
title: "Rsc.Code"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De code of andere informatie over een resource"
type: docs
weight: 210
url: /nl/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

De code of andere informatie over een resource.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Code te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


