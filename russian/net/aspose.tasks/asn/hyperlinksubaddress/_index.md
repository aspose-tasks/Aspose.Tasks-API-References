---
title: "Asn.HyperlinkSubAddress"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Конкретное местоположение в документе гиперссылки, связанной с назначением"
type: docs
weight: 300
url: /ru/net/aspose.tasks/asn/hyperlinksubaddress/
---
## Asn.HyperlinkSubAddress field

Конкретное место в документе гиперссылки, связанной с назначением.

```csharp
public static readonly Key<string, AsnKey> HyperlinkSubAddress;
```

## Примечания

Полный адрес (Hyperlink Href в Microsoft Project) гиперссылки представляет собой конкатенацию HyperlinkAddress и HyperlinkSubAddress.

## Примеры

Показывает, как читать/записывать свойства гиперссылки.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


