---
title: "Prj.MultipleCriticalPaths"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Birden fazla kritik yolun hesaplanıp hesaplanmayacağını belirler"
type: docs
weight: 530
url: /tr/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

Birden fazla kritik yolun hesaplanıp hesaplanmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## Örnekler

Prj.MultipleCriticalPaths özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


