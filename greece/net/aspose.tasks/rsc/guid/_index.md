---
title: "Rsc.Guid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Περιέχει τον παραγόμενο μοναδικό κωδικό αναγνώρισης για τον πόρο"
type: docs
weight: 310
url: /el/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Περιέχει τον παραγόμενο μοναδικό κωδικό αναγνώρισης για τον πόρο.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


