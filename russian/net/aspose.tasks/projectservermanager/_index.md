---
title: "Класс ProjectServerManager"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectServerManager. Класс, предоставляющий методы для чтения и выполнения операций над проектами в указанной учётной записи Project Online или в указанном локальном экземпляре Project Server. Поддерживаются версии Project Server 2016 и 2019."
type: docs
weight: 1500
url: /ru/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

Класс, который предоставляет методы для чтения и выполнения операций над проектами в указанной учётной записи Project Online или в указанном локальном экземпляре Project Server (поддерживаются версии Project Server 2016 и 2019).

```csharp
public sealed class ProjectServerManager
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Инициализирует новый экземпляр класса `ProjectServerManager`. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Создаёт новый проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Создает новый проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Получает проект с указанным GUID из учетной записи Project Online \ экземпляра Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Получает список проектов из хранилища 'Working' текущей учетной записи Project Online \ экземпляра Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Получает двоичные данные проекта для целей устранения неполадок. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. Существующий проект будет перезаписан. |

## События

| Имя | Описание |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Событие, которое вызывается при отправке веб‑запроса к веб‑API Project Server. |

## Примеры

Показывает, как использовать менеджер Project Server для создания нового проекта с предопределенными параметрами сохранения в Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


