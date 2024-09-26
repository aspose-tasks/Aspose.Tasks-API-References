---
title: Rsc.Hyperlink
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The title or explanatory text of a hyperlink associated with a resource
type: docs
weight: 320
url: /net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

The title or explanatory text of a hyperlink associated with a resource.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

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


