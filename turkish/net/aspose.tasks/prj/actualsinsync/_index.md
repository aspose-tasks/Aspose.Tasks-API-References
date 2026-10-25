---
title: "Prj.ActualsInSync"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Tüm gerçek işlerin proje ile senkronize edilip edilmediğini belirler"
type: docs
weight: 10
url: /tr/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

Tüm gerçek işlerin proje ile senkronize edilip edilmediğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## Örnekler

Prj.ActualsInSync özelliğini okuma/yazma işleminin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


