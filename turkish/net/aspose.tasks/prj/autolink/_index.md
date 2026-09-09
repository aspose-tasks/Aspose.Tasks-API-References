---
title: "Prj.Autolink"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Eklenen veya taşınan görevlerin otomatik olarak bağlanıp bağlanmayacağını belirler"
type: docs
weight: 70
url: /tr/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Ekleme veya taşıma görevlerinin otomatik olarak bağlanıp bağlanmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Örnekler

Prj.Autolink özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


