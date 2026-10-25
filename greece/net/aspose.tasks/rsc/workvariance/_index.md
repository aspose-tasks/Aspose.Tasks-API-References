---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διαφορά μεταξύ της βασικής εργασίας ενός πόρου και της τρέχουσας προγραμματισμένης εργασίας"
type: docs
weight: 710
url: /el/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

Η διαφορά μεταξύ της βασικής εργασίας ενός πόρου και της τρέχουσας προγραμματισμένης εργασίας.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τη διακύμανση εργασίας του πόρου.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


