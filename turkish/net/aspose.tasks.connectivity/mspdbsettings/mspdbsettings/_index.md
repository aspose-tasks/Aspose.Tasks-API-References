---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MspDbSettings yapıcı. MspDbSettings sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

Yeni bir örnek oluşturur [`MspDbSettings`](../) sınıfını.

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connectionString | Dize | belirtilen bağlantı dizesi. |
| projectGuid | Guid | okunacak projenin belirtilen guid'i. |

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

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


