---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει εάν ένας πόρος έχει απενεργοποιηθεί από χρήστη με διαχειριστικά δικαιώματα"
type: docs
weight: 360
url: /el/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Καθορίζει εάν ένας πόρος απενεργοποιήθηκε από χρήστη με διαχειριστικά δικαιώματα.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


