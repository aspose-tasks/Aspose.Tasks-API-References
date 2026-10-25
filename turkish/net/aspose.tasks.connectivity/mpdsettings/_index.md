---
title: "MpdSettings sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Connectivity.MpdSettings sınıfı. MPD formatındaki MS Access veritabanı dosyasından proje verilerini okumak için gerekli seçenekleri ayarlamayı sağlar"
type: docs
weight: 300
url: /tr/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

MPD formatından (MS Access veritabanı dosya formatı) proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir.

```csharp
public class MpdSettings : DbSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | `MpdSettings` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Bağlantı dizesini alır veya ayarlar. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Okunacak projenin kimliğini alır. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Proje yükleme işlemleri sırasında çağrılacak geri aramayı alır veya ayarlar. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Veritabanına bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa, ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory sınıfının bir örneğini elde etmek için kullanılan sağlayıcı sabit adını alır veya ayarlar. Varsayılan değer SqlClient'tır. |

## Örnekler

Veritabanından projenin içe aktarımını kontrol etmek için MPD ayarlarının nasıl kullanılacağını gösterir.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


