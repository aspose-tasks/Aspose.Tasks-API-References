---
title: "Sınıf PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.PrimaveraXerReader sınıfı. Primavera XER dosyasından Proje UID'lerini okumak için bir okuyucu temsil eder."
type: docs
weight: 1390
url: /tr/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Primavera XER dosyasından Proje UID'lerini okumak için bir okuyucuyu temsil eder.

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | `PrimaveraXerReader` sınıfının yeni bir örneğini başlatır. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | `PrimaveraXerReader` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Projenin kısa bilgi nesnelerinin bir listesini döndür. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Projelerin benzersiz tanımlayıcılarının bir listesini döndür. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Belirtilen benzersiz tanımlayıcıya sahip projeyi yükler. |

## Örnekler

Bir Primavera XER dosyasından kısa projelerin bilgilerini nasıl inceleyeceğinizi gösterir.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Ayrıca Bakınız

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


