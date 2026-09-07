---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή συνόλου εργασιών"
type: docs
weight: 610
url: /el/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή συνόλου εργασιών.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


