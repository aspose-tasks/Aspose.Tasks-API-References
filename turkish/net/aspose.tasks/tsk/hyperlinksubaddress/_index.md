---
title: "Tsk.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevle ilişkili bir köprüdeki belgedeki belirli konum"
type: docs
weight: 510
url: /tr/net/aspose.tasks/tsk/hyperlinksubaddress/
---
## Tsk.HyperlinkSubAddress field

Görevle ilişkili bir köprünün belge içindeki belirli konumu.

```csharp
public static readonly Key<string, TaskKey> HyperlinkSubAddress;
```

## Açıklamalar

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

## Örnekler

Tsk.Hyperlink özelliklerini okuma/yazma nasıl yapılacağını gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


