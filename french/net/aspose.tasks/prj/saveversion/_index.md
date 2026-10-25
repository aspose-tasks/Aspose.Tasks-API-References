---
title: "Prj.SaveVersion"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La version de Microsoft Office Project à partir de laquelle un fichier de projet a été enregistré"
type: docs
weight: 620
url: /fr/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

La version de Microsoft Office Project à partir de laquelle le fichier de projet a été enregistré.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Exemples

Montre comment vérifier la version d'enregistrement du projet et la date d'enregistrement.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Afficher la version du projet
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


