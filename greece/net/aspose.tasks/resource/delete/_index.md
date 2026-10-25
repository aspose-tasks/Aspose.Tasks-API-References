---
title: "Resource.Delete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Resource. Διαγράφει έναν πόρο και τις αναθέσεις του από το έργο"
type: docs
weight: 810
url: /el/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Διαγράφει έναν πόρο και τις αναθέσεις του από το έργο.

```csharp
public void Delete()
```

## Παραδείγματα

Δείχνει πώς να διαγράψετε έναν πόρο.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// διαγράψτε τον πόρο
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Δείτε επίσης

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


