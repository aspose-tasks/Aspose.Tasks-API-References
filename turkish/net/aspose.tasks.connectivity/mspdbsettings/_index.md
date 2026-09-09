---
title: "Sınıf MspDbSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Connectivity.MspDbSettings sınıfı. MS Project Server veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamayı sağlar"
type: docs
weight: 310
url: /tr/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

MS Project Server veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir.

```csharp
public class MspDbSettings : DbSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | `MspDbSettings` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Bağlantı dizesini alır veya ayarlar. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Okunacak projenin GUID'ini alır. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Proje yükleme işlemleri sırasında çağrılacak geri aramayı alır veya ayarlar. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Veritabanına bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa, ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory sınıfının bir örneğini elde etmek için kullanılan sağlayıcı sabit adını alır veya ayarlar. Varsayılan değer SqlClient'tır. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | MS Project Server'ın şemasını alır veya ayarlar. Varsayılan değer "pub"dır. |

## Örnekler

Bir veritabanından proje nasıl içe aktarılır gösterir.

```csharp
try
{
    // Bağlantı dizesi oluştur
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // MS veritabanından yüklemek için ayarları oluştur
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### Ayrıca Bakınız

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


