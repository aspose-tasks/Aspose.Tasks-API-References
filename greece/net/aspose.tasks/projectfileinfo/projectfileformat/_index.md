---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectFileInfo ιδιότητα. Λαμβάνει μορφή αρχείου έργου"
type: docs
weight: 40
url: /el/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Επιστρέφει τη μορφή του αρχείου έργου.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


