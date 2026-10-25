---
title: "PrimaveraXmlReader sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.PrimaveraXmlReader sınıfı. Primavera Xml dosyasından Proje UID'lerini almayı sağlayan bir okuyucu temsil eder"
type: docs
weight: 1400
url: /tr/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Primavera Xml dosyasından Proje UID'lerini almayı sağlayan bir okuyucuyu temsil eder.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | `PrimaveraXmlReader` sınıfının yeni bir örneğini başlatır. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | `PrimaveraXmlReader` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Projenin kısa bilgi nesnelerinin bir listesini döndür. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Projelerin benzersiz tanımlayıcılarının bir listesini döndür. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Belirtilen benzersiz tanımlayıcıya sahip projeyi yükler. |

## Örnekler

Bir Primavera XML dosyasından kısa projelerin bilgilerini nasıl inceleyeceğinizi gösterir.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Ayrıca Bakınız

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


