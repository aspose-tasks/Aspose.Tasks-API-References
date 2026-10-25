---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. Durum tarihinden sonra başlaması planlanan ancak daha erken başlayan görevlerin kalan bölümlerinin başlangıcının durum tarihine geri taşınıp taşınmayacağını belirler."
type: docs
weight: 510
url: /tr/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Durum tarihinden önce başlamış ancak durum tarihinden sonra başlaması planlanan görevlerin kalan bölümlerinin başlangıcının durum tarihine geri taşınıp taşınmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Örnekler

Prj.MoveRemainingStartsBack özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


