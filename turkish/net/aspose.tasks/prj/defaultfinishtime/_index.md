---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yeni görevlerin varsayılan bitiş zamanı"
type: docs
weight: 230
url: /tr/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

Yeni görevlerin varsayılan bitiş zamanı.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Örnekler

Prj.DefaultFinishTime özelliğini nasıl okuma/yazma yapacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


