---
title: "Prj.LastSaved"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date à laquelle le projet a été enregistré pour la dernière fois. Enregistré au format UTC dans les fichiers mpp. Type DateTime."
type: docs
weight: 440
url: /fr/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

La date à laquelle un projet a été enregistré pour la dernière fois. Enregistrée au format UTC dans les fichiers mpp. Type DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


