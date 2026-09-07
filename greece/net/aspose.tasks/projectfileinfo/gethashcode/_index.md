---
title: "ProjectFileInfo.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectFileInfo μέθοδος. Επιστρέφει τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης ProjectFileInfo"
type: docs
weight: 60
url: /el/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Επιστρέφει τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πληροφορίες του αρχείου έργου.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


