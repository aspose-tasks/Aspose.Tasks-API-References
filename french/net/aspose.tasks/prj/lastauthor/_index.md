---
title: "Prj.LastAuthor"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Dernier auteur du projet"
type: docs
weight: 420
url: /fr/net/aspose.tasks/prj/lastauthor/
---
## Prj.LastAuthor field

Dernier auteur du projet.

```csharp
public static readonly Key<string, PrjKey> LastAuthor;
```

## Exemples

Montre comment définir les métadonnées du projet.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Définir les informations du projet
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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


