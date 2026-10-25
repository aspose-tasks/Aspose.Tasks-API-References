---
title: "Prj.Revision"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο αριθμός των φορών που αποθηκεύτηκε το έργο"
type: docs
weight: 610
url: /el/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

Ο αριθμός των φορών που αποθηκεύτηκε ένα έργο.

```csharp
public static readonly Key<int, PrjKey> Revision;
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μεταπληροφορίες έργου.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Ορίστε πληροφορίες έργου
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


