---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ποσό του υπόλοιπου προγραμματισμένου υπερωριακού χρόνου"
type: docs
weight: 600
url: /el/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

Το ποσό των υπόλοιπων προγραμματισμένων υπερωριών.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


