---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerCredentials constructor. Initialiseert een nieuwe instantie van de ProjectServerCredentials‑klasse met behulp van de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA‑Project Web Access‑site van SharePoint"
type: docs
weight: 10
url: /nl/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Initialiseert een nieuwe instantie van de [`ProjectServerCredentials`](../) klasse met behulp van de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA‑site (Project Web Access) van SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| siteUrl | String | De URL van de PWA (Project Web Access) API van Project Online. |
| authToken | String | Het autorisatietoken (SPOIDCRL) voor de PWA (Project Web Access) site van SharePoint. |

## Opmerkingen

Gebruik deze constructor om verbinding te maken met ProjectOnline wanneer je al een AuthToken hebt voor je SharePoint Online‑site.

## Voorbeelden

Toont hoe u Project Server‑referenties met SharePointOnlineCredentials gebruikt om een project te maken in Microsoft Project Online.

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

### Zie ook

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`ProjectServerCredentials`](../)‑klasse met de URL van de SharePoint‑site, gebruikersnaam en wachtwoord.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| siteUrl | String | De URL van de PWA (Project Web Access) API van Project Online. |
| userName | String | De gebruikersnaam voor de SharePoint‑site. |
| password | String | Het wachtwoord voor de SharePoint‑site. |

## Opmerkingen

Gebruik deze constructor om verbinding te maken met ProjectOnline. Houd er rekening mee dat legacy‑authenticatie moet worden ingeschakeld in je Azure‑portal en Office 365‑admincentrum.

## Voorbeelden

Toont hoe projectserverreferenties te gebruiken om een lijst met projecten op te halen uit Microsoft Project Online.

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

### Zie ook

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Initialiseert een nieuw exemplaar van de [`ProjectServerCredentials`](../)‑klasse met de URL van het Project Web Access‑eindpunt en netwerkreferenties.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| siteUrl | String | De URL van het Project Web Access‑eindpunt. |
| referenties | NetworkCredential | De referenties die worden gebruikt om in te loggen op het Project Web Access‑eindpunt. |

## Opmerkingen

Gebruik deze constructor om verbinding te maken met een on‑premise‑instantie van Project Server via PWA.

## Voorbeelden

In dit voorbeeld wordt de instantie van de [`ProjectServerManager`](../../projectservermanager/)‑klasse gebruikt om een lijst met projecten te lezen van een Project Server‑instantie die zich bevindt op http://project_server_instance.local

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

Toont hoe je Project Server‑referenties met netwerkreferenties kunt gebruiken om een project te lezen van een on‑premise‑instantie van Project Server.

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

### Zie ook

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


