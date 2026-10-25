---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ProjectServerCredentials constructor. Inizializza una nuova istanza della classe ProjectServerCredentials utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il sito PWA Project Web Access di SharePoint"
type: docs
weight: 10
url: /it/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Inizializza una nuova istanza della classe [`ProjectServerCredentials`](../) utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il PWA (Project Web Access) di SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| siteUrl | Stringa | L'URL dell'API PWA (Project Web Access) di Project Online. |
| authToken | Stringa | Il token di autorizzazione (SPOIDCRL) per il sito PWA (Project Web Access) di SharePoint. |

## Osservazioni

Utilizza questo costruttore per connetterti a ProjectOnline quando disponi già di AuthToken per il sito SharePoint Online.

## Esempi

Mostra come utilizzare le credenziali di Project Server con SharePointOnlineCredentials per creare un progetto in Microsoft Project Online.

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

### Vedi anche

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Inizializza una nuova istanza della classe [`ProjectServerCredentials`](../) usando l'URL del sito SharePoint, nome utente e password.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| siteUrl | Stringa | L'URL dell'API PWA (Project Web Access) di Project Online. |
| userName | Stringa | Il nome utente per il sito SharePoint. |
| password | Stringa | La password per il sito SharePoint. |

## Osservazioni

Utilizza questo costruttore per connetterti a ProjectOnline. Nota che l'autenticazione legacy deve essere abilitata nel tuo portale Azure e nel centro amministrativo di Office 365.

## Esempi

Mostra come utilizzare le credenziali del server di progetto per recuperare l'elenco dei progetti da Microsoft Project Online.

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

### Vedi anche

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Inizializza una nuova istanza della classe [`ProjectServerCredentials`](../) usando l'URL del punto di accesso Project Web Access e le credenziali di rete.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| siteUrl | Stringa | L'URL del punto di accesso project web access. |
| credenziali | NetworkCredential | Le credenziali utilizzate per accedere al punto di accesso Project Web Access. |

## Osservazioni

Utilizza questo costruttore per connetterti all'istanza on-premise di Project Server tramite PWA.

## Esempi

In questo esempio l'istanza della classe [`ProjectServerManager`](../../projectservermanager/) viene utilizzata per leggere un elenco di progetti dall'istanza di Project Server situata all'indirizzo http://project_server_instance.local

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

Mostra come utilizzare le credenziali di Project Server con le credenziali di rete per leggere un progetto dall'istanza on-premise di Project Server.

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

### Vedi anche

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


