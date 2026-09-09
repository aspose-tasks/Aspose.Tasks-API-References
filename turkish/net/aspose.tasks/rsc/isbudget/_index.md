---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir iş malzemesi veya maliyet kaynağının bütçe kaynağı olup olmadığını belirler"
type: docs
weight: 380
url: /tr/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Bir iş, malzeme veya maliyet kaynağının bütçe kaynağı olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Örnekler

Rsc.IsBudget özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


