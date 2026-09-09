---
title: "PrimaveraDbSettings sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings sınıfı. Primavera veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamayı sağlar"
type: docs
weight: 320
url: /tr/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Primavera veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | `PrimaveraDbSettings` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Bağlantı dizesini alır veya ayarlar. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Okunacak projenin kimliğini alır. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Proje yükleme işlemleri sırasında çağrılacak geri aramayı alır veya ayarlar. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Veritabanına bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa, ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory sınıfının bir örneğini elde etmek için kullanılan sağlayıcı sabit adını alır veya ayarlar. Varsayılan değer SqlClient'tır. |

## Örnekler

Bir Primavera veritabanından projenin nasıl içe aktarılacağını gösterir.

```csharp
// Bağlantı dizesi ve proje kimliği ile PrimaveraDbSettings sınıfının yeni bir örneğini başlat
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502 ile projeyi okuyun
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

Primavera veritabanından projelerin kısa bilgilerini nasıl alacağınızı gösterir.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Ayrıca Bakınız

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


