---
title: "Rsc.Code"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο κώδικας ή άλλες πληροφορίες σχετικά με έναν πόρο."
type: docs
weight: 210
url: /el/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Ο κώδικας ή άλλες πληροφορίες σχετικά με έναν πόρο.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


