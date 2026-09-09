---
title: "Enum CostAccrualType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CostAccrualType enum. Bir birikimli maliyetin türünü belirtir."
type: docs
weight: 350
url: /tr/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Tahakkuk maliyetinin tipini belirtir.

```csharp
public enum CostAccrualType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız değerin, alanın orijinal proje dosyasında tanımlı olmadığı anlamına geldiğini gösterir. |
| Start | `0` | Başlangıç maliyet birikim türünü gösterir. |
| Prorated | `1` | Orantılı maliyet birikim türünü gösterir. |
| End | `2` | Bitiş maliyet birikim türünü gösterir. |
| Invalid | `3` | Geçersiz maliyet birikim türünü gösterir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Kaynak standart ve fazla mesai maliyetlerinin ne zaman tahsil edileceğini veya birikeceğini gösterir (birikim yöntemi: Bir kaynağın maliyetinin ne zaman ortaya çıktığını ve gerçek maliyetlerin bir projeye ne zaman yansıtıldığını belirler. Maliyetleri bir görevin başlangıcında [Start] veya bitişinde [End] ortaya çıkarabilir veya görevin süresince [Prorated] orantılı olarak dağıtabilirsiniz.), bir görevin maliyetine (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// maliyet birikim türünü ayarla
// Eğer Bitiş seçeneğini seçerseniz, kalan iş sıfır olana kadar maliyetler birikmez.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// projeyle çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


