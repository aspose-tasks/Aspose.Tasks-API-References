---
title: "Sınıf LoadOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.LoadOptions sınıfı. Bir projeyi dosyadan veya akıştan yüklerken ek yük parametreleri belirtmeye olanak tanır"
type: docs
weight: 990
url: /tr/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Bir projeyi dosyadan veya akıştan yüklerken ek yükleme parametreleri belirtmeye izin verir.

```csharp
public class LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LoadOptions](loadoptions/)() | `LoadOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Proje yükleme işlemini iptal etmek için kullanılabilecek bir token alır veya ayarlar. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | HTML, MPX, XER ve Primavera XML formatlarından bir proje okurken kullanılan kodlamayı alır veya ayarlar. Varsayılan kodlama UTF8'dir. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | XML ayrıştırma hatalarını ele almak için bir geri arama yöntemi alır veya ayarlar. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Koruma şifresini alır veya ayarlar. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | [`PrimaveraReadOptions`](../primaverareadoptions/) sınıfının belirtilen bir örneğini alır veya ayarlar; bu, Primavera formatlarının (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir. |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Proje yükleme işlemleri sırasında çağrılacak geri aramayı alır veya ayarlar. Şu anda MPP ve XER formatları için desteklenmektedir. |

## Örnekler

Şifre korumalı projeyi <see cref=\"Aspose.Tasks.LoadOptions\"/> örneği kullanarak nasıl yükleyeceğinizi gösterir.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


