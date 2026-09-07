---
title: "Rsc.Initials"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Τα αρχικά ενός πόρου"
type: docs
weight: 370
url: /el/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Τα αρχικά ενός πόρου.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


