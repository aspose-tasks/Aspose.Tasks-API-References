---
title: "Project.GetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Temel kaydetme zamanını döndürür"
type: docs
weight: 1090
url: /tr/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Temel kaydetme zamanını döndürür.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baselineNumber | BaselineType | Temel çizginin numarası [`BaselineType`](../../baselinetype/). |

### Dönüş Değeri

Temel çizginin son kaydetme tarihi ve saati.

## Açıklamalar

Temel kaydedilmemişse DateTime.MinValue değerini döndürür.

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


