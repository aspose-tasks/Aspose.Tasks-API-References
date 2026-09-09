---
title: "Enum TaskLinkType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskLinkType enum. Görev bağımlılığının türünü belirtir"
type: docs
weight: 2440
url: /tr/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Görev bağımlılıklarının türünü belirtir.

```csharp
public enum TaskLinkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| FinishToFinish | `0` | Bitiş-Bitiş ilişkisi |
| FinishToStart | `1` | Bitiş-Başlangıç ilişkisi |
| StartToFinish | `2` | Başlangıç-Bitiş ilişkisi |
| StartToStart | `3` | Başlangıç-Başlangıç ilişkisi |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


