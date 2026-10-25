---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource property. Haalt het bovenliggende project op voor deze container"
type: docs
weight: 600
url: /nl/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Haalt het bovenliggende project op voor deze container.

```csharp
public Project ParentProject { get; }
```

## Voorbeelden

Toont hoe het bovenliggende project van resource te gebruiken.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Stel een werk in voor de resource door het standaard projectwerktijd-eenheidstype te gebruiken.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Zie ook

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


