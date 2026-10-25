---
title: "Rsc.HyperlinkAddress"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο"
type: docs
weight: 330
url: /el/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

Η διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Παρατηρήσεις

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του hyperlink είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

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


