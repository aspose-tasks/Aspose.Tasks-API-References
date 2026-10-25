---
title: "Prj.Author"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο δημιουργός ενός έργου."
type: docs
weight: 40
url: /el/net/aspose.tasks/prj/author/
---
## Prj.Author field

Ο συγγραφέας ενός έργου.

```csharp
public static readonly Key<string, PrjKey> Author;
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


