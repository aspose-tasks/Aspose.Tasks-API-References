---
title: ProjectServerManager.GetProjectRawData
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager method. Gets the projects binary data for troubleshooting purposes
type: docs
weight: 60
url: /net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Gets the project's binary data for troubleshooting purposes.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectGuid | Guid | The Guid of the project to read. |

### Return Value

Stream containing raw project's data.

## Examples

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid of project you are trying to get.
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

Shows how to retrieve project's raw data from Microsoft Project Online for troubleshooting purposes.

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

    // The user can read the project as raw data stream for troubleshooting purposes.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // you can pass the resulting file to support.
}
```

### See Also

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


