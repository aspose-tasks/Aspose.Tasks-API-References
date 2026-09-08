---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectServerManager. Получает двоичные данные проекта для целей устранения неполадок."
type: docs
weight: 60
url: /ru/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Получает двоичные данные проекта для целей устранения неполадок.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectGuid | Guid | Guid проекта, который нужно прочитать. |

### Возвращаемое значение

Поток, содержащий необработанные данные проекта.

## Примеры

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// GUID проекта, который вы пытаетесь получить.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

Показывает, как получить необработанные данные проекта из Microsoft Project Online для целей устранения неполадок.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // Пользователь может читать проект как поток необработанных данных для целей устранения неполадок.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // Вы можете передать полученный файл в службу поддержки.
}
```

### См. также

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


