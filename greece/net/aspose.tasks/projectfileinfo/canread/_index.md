---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectFileInfo ιδιότητα. Λαμβάνει τιμή που υποδεικνύει εάν ορίζονται μπορούν Aspose.Tasks να επεξεργαστούν το αρχείο έργου"
type: docs
weight: 10
url: /el/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Επιστρέφει μια τιμή που υποδεικνύει εάν το Aspose.Tasks μπορεί να επεξεργαστεί το αρχείο έργου.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


