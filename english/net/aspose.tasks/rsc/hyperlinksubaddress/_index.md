---
title: Rsc.HyperlinkSubAddress
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The specific location in a document in a hyperlink associated with a task
type: docs
weight: 340
url: /net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

The specific location in a document in a hyperlink associated with a task.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
```

## Remarks

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

## Examples

Shows how to read/write resources hyperlink properties.

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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


