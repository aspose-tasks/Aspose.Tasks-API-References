---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DbSettings özelliği. Bağlantı dizesini alır veya ayarlar."
type: docs
weight: 10
url: /tr/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Bağlantı dizesini alır veya ayarlar.

```csharp
public string ConnectionString { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


