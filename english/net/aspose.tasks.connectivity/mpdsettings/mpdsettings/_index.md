---
title: MpdSettings.MpdSettings
second_title: Aspose.Tasks for .NET API Reference
description: MpdSettings constructor. Initializes a new instance of the MpdSettings class
type: docs
weight: 10
url: /net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Initializes a new instance of the [`MpdSettings`](../) class.

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connectionString | String | the specified connection string. |
| projectId | Int32 | the specified id of a project to read. |

## Examples

Shows how to read a project from an MPD file.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


