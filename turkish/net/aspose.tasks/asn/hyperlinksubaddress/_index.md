---
title: "Asn.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Atama ile ilişkili bir köprünün bir belgedeki belirli konumu"
type: docs
weight: 300
url: /tr/net/aspose.tasks/asn/hyperlinksubaddress/
---
## Asn.HyperlinkSubAddress field

Bir atama ile ilişkili bir köprü bağlantısındaki belgenin belirli konumu.

```csharp
public static readonly Key<string, AsnKey> HyperlinkSubAddress;
```

## Açıklamalar

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

## Örnekler

Köprü özelliklerinin nasıl okunup yazılacağını gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


