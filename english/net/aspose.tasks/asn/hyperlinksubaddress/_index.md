---
title: Asn.HyperlinkSubAddress
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The specific location in a document in a hyperlink associated with an assignment
type: docs
weight: 300
url: /net/aspose.tasks/asn/hyperlinksubaddress/
---
## Asn.HyperlinkSubAddress field

The specific location in a document in a hyperlink associated with an assignment.

```csharp
public static readonly Key<string, AsnKey> HyperlinkSubAddress;
```

## Remarks

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

## Examples

Shows how to read/write hyperlink properties.

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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


