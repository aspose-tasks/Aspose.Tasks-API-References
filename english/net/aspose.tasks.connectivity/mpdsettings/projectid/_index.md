---
title: MpdSettings.ProjectId
second_title: Aspose.Tasks for .NET API Reference
description: MpdSettings property. Gets id of the project to read
type: docs
weight: 20
url: /net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Gets id of the project to read.

```csharp
public int ProjectId { get; }
```

## Examples

Shows how to use MPD settings to control import of project from the database.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


