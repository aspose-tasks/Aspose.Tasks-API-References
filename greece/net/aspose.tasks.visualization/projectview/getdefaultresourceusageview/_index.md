---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectView. Περιλαμβάνει στήλες πόρων Uid, όνομα, έναρξη, λήξη και εργασία"
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Περιλαμβάνει στήλες Uid, name, start, finish και work resource.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Τιμή Επιστροφής

μια προβολή που περιέχει μια λίστα των [`ResourceViewColumn`](../../resourceviewcolumn/).

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή χρήσης πόρων.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Δείτε επίσης

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


