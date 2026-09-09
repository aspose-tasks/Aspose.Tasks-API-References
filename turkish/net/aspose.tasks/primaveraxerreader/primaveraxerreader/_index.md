---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraXerReader yapıcı. PrimaveraXerReader sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

[`PrimaveraXerReader`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| xerFilePath | Dize | Primavera projesinin veya projelerinin bulunduğu .xer dosyasının yolu. |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

[`PrimaveraXerReader`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Primavera XER içeriğine sahip akış. |

### Ayrıca Bakınız

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


