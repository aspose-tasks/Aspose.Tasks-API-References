---
title: "Sınıf PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.PrimaveraReadOptions sınıfı. Primavera Xml veya Primavera Xer dosyalarını okurken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 1370
url: /tr/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Primavera Xml veya Primavera Xer dosyaları okunurken ek seçenekler belirtmeye olanak tanır.

```csharp
public class PrimaveraReadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Yeni bir `PrimaveraReadOptions` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Varlıkların orijinal benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı alır veya ayarlar. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Birden fazla proje içeren dosyadan okunacak projenin UID'sini alır veya ayarlar. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Temel hat projelerinin yüklenip yüklenmeyeceğini belirten bir bayrağı alır veya ayarlar. Varsayılan değer doğrudur. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | XER formatından okunan tanımsız kısıtlamalara sahip görevlerin işlenmesinde kullanılan davranışı belirler. |

## Örnekler

Birden fazla proje içeren Primavera XML veya Primavera XER dosyasından bir projenin nasıl okunacağını gösterir.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Özel UID'ye sahip projeyi döndürür
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


