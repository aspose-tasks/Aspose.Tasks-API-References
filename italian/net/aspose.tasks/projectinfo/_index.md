---
title: "Classe ProjectInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectInfo. Breve informazioni sul progetto pubblicato disponibile su Project Online"
type: docs
weight: 1470
url: /it/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Breve informazioni sul progetto pubblicato disponibile su Project Online.

```csharp
public sealed class ProjectInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Inizializza una nuova istanza della classe `ProjectInfo`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Restituisce la data e l'ora in cui il progetto è stato creato. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Restituisce la descrizione del progetto. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Restituisce l'identificatore univoco del progetto. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Restituisce un valore che indica se il progetto è stato estratto. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Restituisce la data più recente in cui il progetto è stato pubblicato. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Restituisce la data più recente in cui il progetto è stato salvato. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Restituisce il nome del progetto. |

## Esempi

Mostra come leggere le informazioni sui progetti da Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// leggi le informazioni del progetto
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


