---
title: "Rsc.Hyperlink"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο"
type: docs
weight: 320
url: /el/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

Ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες υπερσυνδέσμων των πόρων.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


