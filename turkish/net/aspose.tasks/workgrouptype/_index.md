---
title: "Enum WorkGroupType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkGroupType enum. Bir iş grubunun tipini belirtir"
type: docs
weight: 3620
url: /tr/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Bir iş grubunun türünü belirtir.

```csharp
public enum WorkGroupType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Varsayılan iş grubu tipini gösterir. |
| None | `1` | Hiçbiri iş grubu tipini gösterir. |
| Email | `2` | E-posta iş grubu tipini gösterir. |
| Web | `3` | Web iş grubu tipini gösterir. |

## Örnekler

Bir kaynağın iş grubunun nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


