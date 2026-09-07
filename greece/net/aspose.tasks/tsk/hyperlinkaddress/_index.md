---
title: "Tsk.HyperlinkAddress"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία"
type: docs
weight: 500
url: /el/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

Η διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Παρατηρήσεις

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του hyperlink είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες Tsk.Hyperlink.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


