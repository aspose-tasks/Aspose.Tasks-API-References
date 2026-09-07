---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο τύπος μιας ομάδας εργασίας στην οποία ανήκει ένας πόρος."
type: docs
weight: 700
url: /el/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Ο τύπος μιας ομάδας εργασίας στην οποία ανήκει ένας πόρος.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


