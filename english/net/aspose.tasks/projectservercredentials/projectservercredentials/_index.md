---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerCredentials constructor. Initializes a new instance of the ProjectServerCredentials class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoints PWA Project Web Access site
type: docs
weight: 10
url: /net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Initializes a new instance of the [`ProjectServerCredentials`](../) class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA (Project Web Access) site.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parameter | Type | Description |
| --- | --- | --- |
| siteUrl | String | The URL of PWA (Project Web Access) API of Project Online. |
| authToken | String | The authorization token (SPOIDCRL) for SharePoint's PWA (Project Web Access) site. |

## Remarks

Use this constructor to connect to ProjectOnline when you already have AuthToken for your SharePoint Online site.

## Examples

Shows how to use Project Server credentials with SharePointOnlineCredentials to create project in Microsoft Project Online.

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

### See Also

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Initializes a new instance of the [`ProjectServerCredentials`](../) class using URL of SharePoint site, user name and password.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| siteUrl | String | The URL of PWA (Project Web Access) API of Project Online. |
| userName | String | The user name for the SharePoint site. |
| password | String | The password for the SharePoint site. |

## Remarks

Use this constructor to connect to ProjectOnline. Please note that legacy authentication should be enabled in your Azure portal and Office 365 Admin center.

## Examples

Shows how to use project server credentials to retrieve list of project from Microsoft Project Online.

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

### See Also

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Initializes a new instance of the [`ProjectServerCredentials`](../) class using URL of Project Web Access endpoint and network credentials.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parameter | Type | Description |
| --- | --- | --- |
| siteUrl | String | The URL of project web access endpoint. |
| credentials | NetworkCredential | The credentials used to login to Project Web Access endpoint. |

## Remarks

Use this constructor to connect to on-premise instance of Project Server via PWA.

## Examples

In this example the instance of [`ProjectServerManager`](../../projectservermanager/) class is used to read a list of project from Project Server instance located at http://project_server_instance.local

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

Shows how to use Project Server credentials with network credentials to read a project from on-premise instance of Project Server.

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

### See Also

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


