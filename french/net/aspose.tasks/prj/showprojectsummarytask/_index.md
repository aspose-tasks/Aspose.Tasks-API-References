---
title: "Prj.ShowProjectSummaryTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine s'il faut afficher les informations récapitulatives d'un projet complet sur une seule ligne avec sa propre barre de tâche récapitulative en haut de la vue du diagramme de Gantt"
type: docs
weight: 640
url: /fr/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Détermine si les informations récapitulatives d'un projet complet doivent être affichées sur une seule ligne avec sa propre barre de tâche récapitulative en haut de la vue du diagramme de Gantt.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Exemples

Montre comment lire/écrire la propriété Prj.ShowProjectSummaryTask.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


