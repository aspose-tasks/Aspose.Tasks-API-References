---
title: "Класс ProjectServerCredentials"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectServerCredentials. Учётные данные, которые используются для подключения к Project Online или к локальному экземпляру Project Server."
type: docs
weight: 1490
url: /ru/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Учётные данные, которые используются для подключения к Project Online или локальному экземпляру Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Инициализирует новый экземпляр класса `ProjectServerCredentials`, используя URL конечной точки Project Web Access и сетевые учётные данные. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Инициализирует новый экземпляр класса `ProjectServerCredentials`, используя URL сайта SharePoint и действительный токен авторизации SPOIDCRL для сайта PWA (Project Web Access) SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Инициализирует новый экземпляр класса `ProjectServerCredentials`, используя URL сайта SharePoint, имя пользователя и пароль. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Получает токен авторизации для экземпляра SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Получает URL PWA на сайте SharePoint или URL локального Project Server. Например, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Получает имя пользователя для сайта SharePoint. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Возвращает строковое представление этого экземпляра. |

## Примеры

Показывает, как использовать учётные данные сервера проекта для получения списка проектов из Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


