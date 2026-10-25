---
title: "GetProjectUids"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Projelerin benzersiz tanımlayıcılarının bir listesini döndürür."
type: docs
weight: 20
url: /tr/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

Projelerin benzersiz tanımlayıcılarının bir listesini döndür.

```csharp
public List<int> GetProjectUids()
```

### Dönüş Değeri

Projelerin benzersiz tanımlayıcıları listesi.

### Örnekler

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

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
