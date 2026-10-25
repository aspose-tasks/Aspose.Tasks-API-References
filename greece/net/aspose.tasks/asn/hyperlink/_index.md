---
title: "Asn.Hyperlink"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn πεδίο. Ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με μια ανάθεση"
type: docs
weight: 280
url: /el/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

Ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με μια ανάθεση.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες του υπερσυνδέσμου.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


