---
title: "Prj.MoveRemainingStartsForward"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Daha sonra başlaması planlanan görevlerin kalan bölümlerinin başlangıcının durum tarihine taşınıp taşınmayacağını belirler"
type: docs
weight: 520
url: /tr/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Daha sonra başlaması planlanan görevlerin kalan bölümlerinin başlangıcının durum tarihine yükseltilip yükseltilmeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Örnekler

Prj.MoveRemainingStartsForward özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


