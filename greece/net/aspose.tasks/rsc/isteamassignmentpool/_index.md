---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Δείχνει εάν ο τρέχων πόρος είναι πόρος ομάδας"
type: docs
weight: 430
url: /el/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Εμφανίζει εάν ο τρέχων πόρος είναι πόρος ομάδας.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


