---
title: "Rsc.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία."
type: docs
weight: 340
url: /el/net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

Η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
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


