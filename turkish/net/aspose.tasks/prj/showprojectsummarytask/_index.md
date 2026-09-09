---
title: "Prj.ShowProjectSummaryTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Tüm proje hakkında özet bilgilerin Gantt Şeması görünümünün üst kısmında kendi özet görev çubuğuyla tek bir satırda gösterilip gösterilmeyeceğini belirler"
type: docs
weight: 640
url: /tr/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Tüm proje hakkında özet bilgileri, Gantt Şeması görünümünün üst kısmında kendi özet görev çubuğuyla tek bir satırda gösterilip gösterilmeyeceğini belirler.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Örnekler

Prj.ShowProjectSummaryTask özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


