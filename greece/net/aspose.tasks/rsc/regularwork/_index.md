---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το συνολικό ποσό μη υπερωριακής εργασίας που προγραμματίζεται να εκτελεστεί από τον πόρο."
type: docs
weight: 570
url: /el/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

Το συνολικό ποσό μη υπερωριακής εργασίας που έχει προγραμματιστεί να εκτελεστεί από τον πόρο.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


