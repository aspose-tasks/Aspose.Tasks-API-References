---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Bağlantının tipini alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Bir bağlantının türünü alır veya ayarlar.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Örnekler

Bir görev bağlantısının bağlantı türünü nasıl alıp/ayarlayacağınızı gösterir.

```csharp
var project = new Project();

// Yeni görevler ekle
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Görevleri Bağlantı türü Başlangıç‑Başlangıç olarak ayarlayarak bağla
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Ayrıca Bakınız

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


