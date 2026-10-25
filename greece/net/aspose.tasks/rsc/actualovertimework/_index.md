---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το πραγματικό ποσό υπερωριακής εργασίας που έχει ήδη εκτελεστεί από πόρο που έχει ανατεθεί σε εργασίες."
type: docs
weight: 50
url: /el/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

Το πραγματικό ποσό υπερωριακής εργασίας που έχει ήδη εκτελεστεί από πόρο που έχει ανατεθεί σε εργασίες.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


