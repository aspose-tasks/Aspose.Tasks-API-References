---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ProjectServerCredentials. Инициализирует новый экземпляр класса ProjectServerCredentials, используя URL сайта SharePoint и действительный токен авторизации SPOIDCRL для сайта PWA (Project Web Access) SharePoint"
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Инициализирует новый экземпляр класса [`ProjectServerCredentials`](../), используя URL сайта SharePoint и действительный токен авторизации SPOIDCRL для сайта PWA (Project Web Access) SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | Строка | URL PWA (Project Web Access) API сервиса Project Online. |
| authToken | Строка | Токен авторизации (SPOIDCRL) для сайта PWA (Project Web Access) SharePoint. |

## Примечания

Используйте этот конструктор для подключения к ProjectOnline, когда у вас уже есть AuthToken для вашего сайта SharePoint Online.

## Примеры

Показывает, как использовать учетные данные Project Server вместе с SharePointOnlineCredentials для создания проекта в Microsoft Project Online.

```csharp
try
{
    const string Username = "admin@contoso.onmicrosoft.com";
    const string SecuredPassword = "MyPassword";
    var url = new Uri("https://contoso.sharepoint.com/sites/pwa");
    var project = new Project(DataDir + "Project1.mpp");
    var password = new SecureString();
    foreach (var c in SecuredPassword)
    {
        password.AppendChar(c);
    }

    var onlineCredentials = new SharePointOnlineCredentials(Username, password);
    var projectServerCredentials = new ProjectServerCredentials(url.ToString(), onlineCredentials.GetAuthenticationCookie(url, true));

    Console.WriteLine("Project Server Auth Token: " + projectServerCredentials.AuthToken);
    Console.WriteLine("Project Server Site Url: " + projectServerCredentials.SiteUrl);
    Console.WriteLine("Project Server User Name: " + projectServerCredentials.UserName);

    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Инициализирует новый экземпляр класса [`ProjectServerCredentials`](../), используя URL сайта SharePoint, имя пользователя и пароль.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | Строка | URL PWA (Project Web Access) API сервиса Project Online. |
| userName | Строка | Имя пользователя для сайта SharePoint. |
| password | Строка | Пароль для сайта SharePoint. |

## Примечания

Используйте этот конструктор для подключения к ProjectOnline. Обратите внимание, что устаревшая аутентификация должна быть включена в вашем портале Azure и центре администрирования Office 365.

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

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Инициализирует новый экземпляр класса [`ProjectServerCredentials`](../), используя URL конечной точки Project Web Access и сетевые учетные данные.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | Строка | URL конечной точки Project Web Access. |
| учетные данные | NetworkCredential | Учетные данные, используемые для входа в конечную точку Project Web Access. |

## Примечания

Используйте этот конструктор для подключения к локальному экземпляру Project Server через PWA.

## Примеры

В этом примере экземпляр класса [`ProjectServerManager`](../../projectservermanager/) используется для чтения списка проектов из экземпляра Project Server, расположенного по адресу http://project_server_instance.local

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

Показывает, как использовать учетные данные Project Server с сетевыми учетными данными для чтения проекта из локального экземпляра Project Server.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


