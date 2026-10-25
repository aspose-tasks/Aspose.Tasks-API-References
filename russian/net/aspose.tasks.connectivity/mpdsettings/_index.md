---
title: "Класс MpdSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Connectivity.MpdSettings. Позволяет задать необходимые параметры для чтения данных проекта из файла базы данных MS Access в формате MPD"
type: docs
weight: 300
url: /ru/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Позволяет задать необходимые параметры для чтения данных проекта из формата MPD (формат файлов базы данных MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Инициализирует новый экземпляр класса `MpdSettings`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Получает или задает строку подключения. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Получает идентификатор проекта для чтения. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Получает или задает обратный вызов, который будет вызываться во время операций загрузки проекта. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient. |

## Примеры

Показывает, как использовать настройки MPD для управления импортом проекта из базы данных.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


