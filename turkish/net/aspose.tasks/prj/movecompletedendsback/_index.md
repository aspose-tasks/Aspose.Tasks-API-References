---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Durum tarihinden sonra başlaması planlanan ancak daha erken başlayan görevlerin tamamlanmış bölümlerinin sonunun durum tarihine geri taşınıp taşınmayacağını belirler"
type: docs
weight: 490
url: /tr/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Durum tarihinden sonra başlaması planlanan ancak daha erken başlayan görevlerin tamamlanmış bölümlerinin sonunun durum tarihine geri taşınıp taşınmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Örnekler

Prj.MoveCompletedEndsBack özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


