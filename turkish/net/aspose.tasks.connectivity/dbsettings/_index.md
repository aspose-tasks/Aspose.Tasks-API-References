---
title: "DbSettings sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Connectivity.DbSettings sınıfı. Proje veritabanından okumak için ayarları belirtmeyi sağlar"
type: docs
weight: 290
url: /tr/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Proje veritabanından okumak için ayarları belirtmeye izin verir.

```csharp
public abstract class DbSettings
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Bağlantı dizesini alır veya ayarlar. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Proje yükleme işlemleri sırasında çağrılacak geri aramayı alır veya ayarlar. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Veritabanına bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa, ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory sınıfının bir örneğini elde etmek için kullanılan sağlayıcı sabit adını alır veya ayarlar. Varsayılan değer SqlClient'tır. |

## Örnekler

Bir sağlayıcı adı kullanarak birden fazla proje içeren Primavera XML dosyasından proje nasıl okunur gösterir.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Bağlantı dizesi ve proje kimliği kullanarak Primavera DB Ayarları oluştur
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


