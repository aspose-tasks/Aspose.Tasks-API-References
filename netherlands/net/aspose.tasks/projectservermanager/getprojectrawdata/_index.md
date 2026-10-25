---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager-methode. Haalt de binaire gegevens van het project op voor probleemoplossingsdoeleinden."
type: docs
weight: 60
url: /nl/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Haalt de binaire gegevens van het project op voor probleemoplossingsdoeleinden.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectGuid | Guid | De Guid van het project om te lezen. |

### Retourwaarde

Stream die de ruwe projectgegevens bevat.

## Voorbeelden

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// GUID van het project dat u probeert op te halen.
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

Toont hoe de ruwe gegevens van een project op te halen uit Microsoft Project Online voor probleemoplossingsdoeleinden.

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

    // De gebruiker kan het project lezen als een ruwe gegevensstroom voor probleemoplossingsdoeleinden.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // U kunt het resulterende bestand doorsturen naar de ondersteuning.
}
```

### Zie ook

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


