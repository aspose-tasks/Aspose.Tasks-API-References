---
title: "Prj.Revision"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le nombre de fois où le projet a été enregistré"
type: docs
weight: 610
url: /fr/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

Le nombre de fois où le projet a été enregistré.

```csharp
public static readonly Key<int, PrjKey> Revision;
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


