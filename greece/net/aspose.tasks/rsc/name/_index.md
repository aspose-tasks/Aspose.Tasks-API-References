---
title: "Rsc.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το όνομα ενός πόρου"
type: docs
weight: 460
url: /el/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Το όνομα ενός πόρου.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


