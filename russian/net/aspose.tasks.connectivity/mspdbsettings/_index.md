---
title: "Класс MspDbSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Connectivity.MspDbSettings. Позволяет задать необходимые параметры для чтения данных проекта из базы данных MS Project Server"
type: docs
weight: 310
url: /ru/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Позволяет задать необходимые параметры для чтения данных проекта из базы данных MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Инициализирует новый экземпляр класса `MspDbSettings`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Получает или задает строку подключения. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Получает GUID проекта для чтения. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Получает или задает обратный вызов, который будет вызываться во время операций загрузки проекта. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Получает или задает схему MS Project Server. Значение по умолчанию — "pub". |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


