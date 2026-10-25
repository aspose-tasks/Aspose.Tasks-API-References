---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerCredentials yapıcı. SharePoint sitesinin URL'si ve SharePoint'in PWA Project Web Access sitesi için geçerli SPOIDCRL yetkilendirme belirteci kullanarak ProjectServerCredentials sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

SharePoint sitesinin URL'si ve SharePoint'in PWA (Project Web Access) sitesi için geçerli SPOIDCRL yetkilendirme belirteci kullanarak [`ProjectServerCredentials`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| siteUrl | Dize | Project Online'ın PWA (Project Web Access) API'sinin URL'si. |
| authToken | Dize | SharePoint'in PWA (Project Web Access) sitesi için yetkilendirme belirteci (SPOIDCRL). |

## Açıklamalar

SharePoint Online siteniz için AuthToken'ınız olduğunda ProjectOnline'a bağlanmak için bu yapıcıyı kullanın.

## Örnekler

Project Server kimlik bilgilerini SharePointOnlineCredentials ile kullanarak Microsoft Project Online'da proje oluşturmayı gösterir.

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

### Ayrıca Bakınız

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

SharePoint sitesinin URL'si, kullanıcı adı ve şifre kullanarak [`ProjectServerCredentials`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| siteUrl | Dize | Project Online'ın PWA (Project Web Access) API'sinin URL'si. |
| userName | Dize | SharePoint sitesi için kullanıcı adı. |
| password | Dize | SharePoint sitesi için şifre. |

## Açıklamalar

ProjectOnline'a bağlanmak için bu yapıcıyı kullanın. Lütfen eski kimlik doğrulamanın Azure portalınızda ve Office 365 Yönetim merkezinde etkinleştirilmesi gerektiğini unutmayın.

## Örnekler

Microsoft Project Online'dan proje listesini almak için proje sunucusu kimlik bilgilerinin nasıl kullanılacağını gösterir.

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

### Ayrıca Bakınız

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Project Web Access uç noktasının URL'si ve ağ kimlik bilgilerini kullanarak [`ProjectServerCredentials`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| siteUrl | Dize | Project Web Access uç noktasının URL'si. |
| kimlik bilgileri | NetworkCredential | Project Web Access uç noktasına giriş yapmak için kullanılan kimlik bilgileri. |

## Açıklamalar

PWA üzerinden yerel Project Server örneğine bağlanmak için bu yapıcıyı kullanın.

## Örnekler

Bu örnekte, [`ProjectServerManager`](../../projectservermanager/) sınıfının örneği, http://project_server_instance.local adresinde bulunan Project Server örneğinden proje listesini okumak için kullanılır.

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

Project Server kimlik bilgilerini ağ kimlik bilgileriyle birlikte kullanarak yerel Project Server örneğinden bir proje nasıl okunur gösterir.

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

### Ayrıca Bakınız

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


