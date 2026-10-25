---
title: "ProjectServerManager.CreateNewProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectServerManager. Создает новый проект в экземпляре Project ServerProject Online, используя параметры сохранения по умолчанию."
type: docs
weight: 30
url: /ru/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Создаёт новый проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию.

```csharp
public void CreateNewProject(Project project)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект для сохранения в экземпляр Project Server\Project Online. |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

## Примеры

В этом примере проект загружается из файла .mpp и сохраняется в учетную запись Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Показано, как использовать ProjectServerManager для создания нового проекта в Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Создает новый проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект для сохранения в экземпляр Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Экземпляр класса [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

## Примеры

В этом примере проект загружается из файла .mpp и сохраняется в учетную запись Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


