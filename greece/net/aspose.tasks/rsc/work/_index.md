---
title: "Rsc.Work"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το συνολικό ποσό χρόνου που προγραμματίζεται για έναν πόρο σε μια εργασία."
type: docs
weight: 690
url: /el/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

Το συνολικό ποσό χρόνου που έχει προγραμματιστεί για έναν πόρο σε μια εργασία.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


