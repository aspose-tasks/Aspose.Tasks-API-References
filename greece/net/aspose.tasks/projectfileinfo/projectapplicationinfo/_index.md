---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectFileInfo. Επιστρέφει τις πληροφορίες εφαρμογής του αρχείου έργου"
type: docs
weight: 30
url: /el/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Επιστρέφει πληροφορίες εφαρμογής του αρχείου έργου.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πληροφορίες του αρχείου έργου.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


