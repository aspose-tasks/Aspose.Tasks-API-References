---
title: "MspDbSettings.Schema"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MspDbSettings. Получает или задает схему MS Project Server. Значение по умолчанию — pub"
type: docs
weight: 30
url: /ru/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

Получает или задает схему MS Project Server. Значение по умолчанию — "pub".

```csharp
public string Schema { get; set; }
```

## Примеры

Показывает, как импортировать проект из базы данных.

```csharp
try
{
    // Создать строку подключения
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // создать настройки для загрузки из базы данных MS
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

### См. также

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


