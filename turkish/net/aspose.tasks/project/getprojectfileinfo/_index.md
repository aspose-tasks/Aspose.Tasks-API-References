---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project metodu. Proje dosyası bilgilerini dosyadan okur."
type: docs
weight: 1280
url: /tr/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Dosyadan proje dosyası bilgilerini okur.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | Dize | Proje dosya adı. |

### Dönüş Değeri

Proje dosya bilgisi [`ProjectFileInfo`](../../projectfileinfo/).

## Örnekler

XML dosyasından okunan proje dosyası bilgisinin nasıl okunacağını gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Akıştan proje dosyası bilgilerini alır.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Veri akışı. |

### Dönüş Değeri

Proje dosya bilgisi [`ProjectFileInfo`](../../projectfileinfo/).

## Örnekler

Bir akıştan okunan XML dosyasının proje dosyası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Ayrıca Bakınız

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


