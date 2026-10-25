---
title: "Rsc.Id"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Το αναγνωριστικό θέσης ενός πόρου μέσα στη λίστα των πόρων"
type: docs
weight: 350
url: /el/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

Το αναγνωριστικό θέσης ενός πόρου στη λίστα των πόρων.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


