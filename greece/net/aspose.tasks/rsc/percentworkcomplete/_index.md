---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ποσοστό της ολοκληρωμένης εργασίας σε όλες τις εργασίες"
type: docs
weight: 550
url: /el/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Το ποσοστό της ολοκληρωμένης εργασίας σε όλες τις εργασίες.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε το ποσοστό ολοκλήρωσης εργασίας του πόρου.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Εμφανίζει το ποσοστό ολοκλήρωσης εργασίας για όλους τους πόρους
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


