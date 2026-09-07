---
title: "Resource.Baselines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει ένα αντικείμενο BaselineCollection για αυτό το αντικείμενο. Οι τιμές βάσης για έναν πόρο"
type: docs
weight: 160
url: /el/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Λαμβάνει μια παρουσία του BaselineCollection για αυτό το αντικείμενο. Οι τιμές βάσης για έναν πόρο.

```csharp
public BaselineCollection Baselines { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις βάσεις του πόρου.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Δείτε επίσης

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


