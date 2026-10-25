---
title: "Project.SetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Temel çizgi kaydetme zamanını ayarlar"
type: docs
weight: 1260
url: /tr/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Temel çizgi kaydetme zamanını ayarlar.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baselineNumber | BaselineType | Temel çizginin numarası [`BaselineType`](../../baselinetype/). |
| value | DateTime | Temel çizginin son kaydetme tarihi ve saati. |

## Açıklamalar

Temel çizgi kaydedilmemişse değeri DateTime.MinValue olarak ayarla.

## Örnekler

Projenin temel çizgi kaydetme zamanını okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// temel çizgi kaydetme zamanını ayarla
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Ayrıca Bakınız

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


