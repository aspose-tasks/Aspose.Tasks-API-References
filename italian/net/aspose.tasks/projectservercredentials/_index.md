---
title: "Classe ProjectServerCredentials"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectServerCredentials. Credenziali utilizzate per connettersi a Project Online o a un'istanza on‑premise di Project Server"
type: docs
weight: 1490
url: /it/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Credenziali utilizzate per connettersi a Project Online o all'istanza on-premise di Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Inizializza una nuova istanza della classe `ProjectServerCredentials` utilizzando l'URL del punto di accesso Project Web Access e le credenziali di rete. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Inizializza una nuova istanza della classe `ProjectServerCredentials` utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il sito PWA (Project Web Access) di SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Inizializza una nuova istanza della classe `ProjectServerCredentials` utilizzando l'URL del sito SharePoint, nome utente e password. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Ottiene il token di autorizzazione per l'istanza SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Ottiene l'URL di PWA nel sito SharePoint o l'URL di Project Server on‑premise. Per esempio, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Ottiene il nome utente per il sito SharePoint. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Restituisce una rappresentazione stringa di questa istanza. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


