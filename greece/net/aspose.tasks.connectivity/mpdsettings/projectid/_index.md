---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "MpdSettings property. Λαμβάνει το id του έργου για ανάγνωση."
type: docs
weight: 20
url: /el/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Λαμβάνει το id του έργου για ανάγνωση.

```csharp
public int ProjectId { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις ρυθμίσεις MPD για να ελέγξετε την εισαγωγή του έργου από τη βάση δεδομένων.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


