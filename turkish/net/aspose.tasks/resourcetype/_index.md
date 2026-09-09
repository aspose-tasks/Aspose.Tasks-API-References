---
title: "Enum ResourceType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ResourceType enum. Bir kaynağın türünü belirtir"
type: docs
weight: 1800
url: /tr/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Bir kaynağın türünü belirtir.

```csharp
public enum ResourceType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Material | `0` | Malzeme kaynak türünü gösterir. |
| Work | `1` | İş kaynak türünü gösterir. |
| Cost | `2` | Maliyet kaynak türünü gösterir. |

## Örnekler

Kaynak türleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// bir iş kaynağı ekle
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// bir malzeme kaynağı ekle
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// bir malzeme kaynağı ekle
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// kaynaklarla çalış: görevler oluştur, kaynakları ata ve benzeri...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


