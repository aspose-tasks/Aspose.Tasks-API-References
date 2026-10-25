---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraXmlReader yapıcı. PrimaveraXmlReader sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Yeni bir [`PrimaveraXmlReader`](../) sınıfının örneğini başlatır.

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templatePath | Dize | Primavera Xml projesinin veya projelerinin bulunduğu şablonun yolu |

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

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Yeni bir [`PrimaveraXmlReader`](../) sınıfının örneğini başlatır.

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Primavera Xml içeriği içeren akış. |

## Örnekler

Bir Primavera XML akışından proje nasıl içe aktarılacağını gösterir.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### Ayrıca Bakınız

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


