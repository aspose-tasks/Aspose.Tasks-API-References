---
title: "Asn.Hyperlink"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De titel of verklarende tekst van een hyperlink die aan een toewijzing is gekoppeld"
type: docs
weight: 280
url: /nl/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

De titel of verklarende tekst van een hyperlink die aan een opdracht is gekoppeld.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## Voorbeelden

Toont hoe hyperlink-eigenschappen gelezen/geschreven kunnen worden.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


