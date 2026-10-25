---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraBaseReader yöntemi. Projelerin benzersiz tanımlayıcılarının bir listesini döndürür"
type: docs
weight: 20
url: /tr/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Projelerin benzersiz tanımlayıcılarının bir listesini döndür.

```csharp
public List<int> GetProjectUids()
```

### Dönüş Değeri

Projelerin benzersiz tanımlayıcıları listesi.

## Örnekler

Bir Primavera XML dosyasından proje nasıl içe aktarılacağını gösterir.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Ayrıca Bakınız

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


