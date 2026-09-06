---
title: "Project.DisplayOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient une instance de la classe ProjectDisplayOptions"
type: docs
weight: 380
url: /fr/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Obtient une instance de la classe [`ProjectDisplayOptions`](../../projectdisplayoptions/).

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Exemples

Montre comment ajuster les options d'affichage du projet.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Définir une valeur indiquant s'il faut afficher des avertissements lorsque Project identifie un conflit d'échéancier possible avec une tâche planifiée manuellement.
// Cette option est disponible pour la version Project 2010 et suivantes.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Voir aussi

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


