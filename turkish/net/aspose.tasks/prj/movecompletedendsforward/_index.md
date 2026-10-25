---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Durum tarihinden önce tamamlanması planlanan ancak daha sonra başlayan görevlerin tamamlanmış bölümlerinin sonunun durum tarihine yükseltilip yükseltilmeyeceğini belirler"
type: docs
weight: 500
url: /tr/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Durum tarihinden önce tamamlanması planlanan ancak daha sonra başlayan görevlerin tamamlanmış bölümlerinin sonunun durum tarihine yükseltilip yükseltilmeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Örnekler

Prj.MoveCompletedEndsForward özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


