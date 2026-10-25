---
title: "ITextStyleModificationCallback"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un rappel qui est appelé avant que TextStyle ne soit appliqué à une cellule de tableau."
type: docs
weight: 383
url: /fr/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Représente un rappel qui est appelé avant que TextStyle ne soit appliqué à une cellule de tableau.
## Méthodes

| Méthode | Description |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | La méthode à appeler avant le rendu d'une cellule de tableau pour une ligne de tâche dans les vues suivantes : 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


La méthode à appeler avant le rendu d'une cellule de tableau pour une ligne de tâche dans les vues suivantes : 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | L'objet [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

