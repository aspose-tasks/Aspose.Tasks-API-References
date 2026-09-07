---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectView. Περιλαμβάνει στήλες ανάθεσης UID, όνομα εργασίας, όνομα πόρου, εργασία και διάρκεια"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Περιλαμβάνει στήλες Uid, όνομα εργασίας, όνομα πόρου, εργασία και διάρκεια ανάθεσης.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Τιμή Επιστροφής

μια προβολή που περιέχει μια λίστα των [`AssignmentViewColumn`](../../assignmentviewcolumn/).

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή ανάθεσης.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Δείτε επίσης

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


