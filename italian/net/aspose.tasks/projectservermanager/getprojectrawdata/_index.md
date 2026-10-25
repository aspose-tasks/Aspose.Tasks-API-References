---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectServerManager. Ottiene i dati binari del progetto per scopi di risoluzione dei problemi."
type: docs
weight: 60
url: /it/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Recupera i dati binari del progetto per scopi di risoluzione dei problemi.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectGuid | Guid | Il Guid del progetto da leggere. |

### Valore di ritorno

Stream contenente i dati grezzi del progetto.

## Esempi

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// GUID del progetto che stai tentando di ottenere.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

Mostra come recuperare i dati grezzi del progetto da Microsoft Project Online per scopi di risoluzione dei problemi.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // L'utente può leggere il progetto come stream di dati grezzi per scopi di risoluzione dei problemi.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // puoi inviare il file risultante al supporto.
}
```

### Vedi anche

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


