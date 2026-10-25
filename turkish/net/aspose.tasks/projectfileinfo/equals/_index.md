---
title: "ProjectFileInfo.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectFileInfo yöntemi. Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür."
type: docs
weight: 50
url: /tr/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | ProjectFileInfo | Bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

Belirtilen ProjectFileInfo ve bu örnek aynı dosya biçimine ve uygulama bilgisine sahipse true döndürür.

## Örnekler

Proje dosyası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

Belirtilen ProjectFileInfo ve bu örnek aynı dosya biçimine ve uygulama bilgisine sahipse true döndürür.

## Örnekler

Proje dosyası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


