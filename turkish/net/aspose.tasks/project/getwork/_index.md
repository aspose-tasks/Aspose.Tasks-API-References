---
title: "Project.GetWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project method. Belirtilen Double değer ve varsayılan iş formatı ile Duration nesnesini alır"
type: docs
weight: 1130
url: /tr/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Belirtilen Double değer ve varsayılan iş formatı ile [`Duration`](../../duration/) nesnesini alır.

```csharp
public Duration GetWork(double val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Double | belirtilen double değer. |

### Dönüş Değeri

Duration nesnesi.

## Açıklamalar

Bu yöntem dikkatli kullanılmalıdır çünkü Project.WorkFormat ayarına bağlı olarak farklı süreler döndürür. Örneğin, GetWork(1.0) Project.WorkFormat TimeUnitType.Hour olduğunda 1 saat, Project.WorkFormat TimeUnitType.Day olduğunda 1 gün döndürür.

## Örnekler

Varsayılan iş formatı ile bir işi nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// Projenin varsayılan iş formatı ile bir iş değeri oluştur
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


