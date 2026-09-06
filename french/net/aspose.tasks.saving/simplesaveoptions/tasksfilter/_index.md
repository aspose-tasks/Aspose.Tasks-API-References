---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SimpleSaveOptions. Obtient ou définit la condition utilisée pour filtrer les tâches affichées sur la feuille de tâches Gantt et les graphiques d'utilisation des tâches"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Remarques

Si la valeur n'est pas spécifiée, le filtre par défaut est utilisé, ce qui supprime les tâches non visibles — c.-à-d. les tâches descendantes des tâches réduites.

## Exemples

Montre comment utiliser un filtre de tâches personnalisé lors de l'enregistrement d'un fichier MS Project.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // définir un filtre de tâche pour ignorer la tâche 'Task5' et 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // vérifions le format d'enregistrement
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // enregistrer le projet en tant qu’image
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Exemple de filtre de tâche personnalisé qui peut être utilisé lors de l'enregistrement d'un fichier MS Project (par exemple) au format PDF.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### Voir aussi

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


