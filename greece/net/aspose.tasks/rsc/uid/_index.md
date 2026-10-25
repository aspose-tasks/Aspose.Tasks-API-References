---
title: "Rsc.Uid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το μοναδικό αναγνωριστικό ενός πόρου."
type: docs
weight: 670
url: /el/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

Το μοναδικό αναγνωριστικό ενός πόρου.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


