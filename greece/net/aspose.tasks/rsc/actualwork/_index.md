---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η ποσότητα εργασίας που έχει ήδη ολοκληρωθεί από τον πόρο που έχει ανατεθεί σε εργασίες"
type: docs
weight: 70
url: /el/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

Το ποσό εργασίας που έχει ήδη ολοκληρωθεί από πόρο που έχει ανατεθεί σε εργασίες.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


