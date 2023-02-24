---
title: SaveOptions.TasksFilter
second_title: Référence de l'API Aspose.Tasks pour .NET
description: SaveOptions propriété. Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes de Gantt de feuille de tâches et dutilisation des tâches.
type: docs
weight: 190
url: /fr/net/aspose.tasks.saving/saveoptions/tasksfilter/
---
## SaveOptions.TasksFilter property

Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

### Remarques

Si la valeur n'est pas spécifiée, le filtre par défaut est utilisé et supprime les tâches non visibles, c'est-à-dire les tâches descendantes des tâches réduites.

### Voir également

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SaveOptions](../)
* espace de noms [Aspose.Tasks.Saving](../../saveoptions/)
* Assemblée [Aspose.Tasks](../../../)


