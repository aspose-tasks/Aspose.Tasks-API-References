---
title: "Rsc.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. De naam van een resource"
type: docs
weight: 460
url: /nl/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

De naam van een resource.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Name te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


