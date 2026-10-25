---
title: "ProjectInfo.LastPublishedDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectInfo. Ottiene la data più recente in cui il progetto è stato pubblicato"
type: docs
weight: 60
url: /it/net/aspose.tasks/projectinfo/lastpublisheddate/
---
## ProjectInfo.LastPublishedDate property

Restituisce la data più recente in cui il progetto è stato pubblicato.

```csharp
public DateTime LastPublishedDate { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


