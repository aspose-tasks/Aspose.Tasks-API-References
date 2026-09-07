---
title: "ProjectInfo.IsCheckedOut"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectInfo. Ottiene un valore che indica se il progetto è in checkout"
type: docs
weight: 50
url: /it/net/aspose.tasks/projectinfo/ischeckedout/
---
## ProjectInfo.IsCheckedOut property

Restituisce un valore che indica se il progetto è stato estratto.

```csharp
public bool IsCheckedOut { get; }
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


