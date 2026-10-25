---
title: "Sınıf PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.PrimaveraDbReader sınıfı. Primavera DB'den Proje Bilgisi okumak için bir okuyucuyu temsil eder"
type: docs
weight: 1350
url: /tr/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Primavera DB'den Proje Bilgisi okumak için bir okuyucuyu temsil eder.

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Yeni bir [`PrimaveraXerReader`](../primaveraxerreader/) sınıfı örneği başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Projenin kısa bilgi nesnelerinin bir listesini döndür. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Projelerin benzersiz tanımlayıcılarının bir listesini döndür. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Belirtilen benzersiz tanımlayıcıya sahip projeyi yükler. |

## Örnekler

Primavera veritabanından projelerin kısa bilgilerini nasıl alacağınızı gösterir.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Ayrıca Bakınız

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


