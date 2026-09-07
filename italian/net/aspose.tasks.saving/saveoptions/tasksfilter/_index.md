---
title: "TasksFilter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta la condizione utilizzata per filtrare le attività renderizzate nel foglio delle attività Gantt e nei grafici di utilizzo delle attività."
type: docs
weight: 190
url: /it/net/aspose.tasks.saving/saveoptions/tasksfilter/
---
## SaveOptions.TasksFilter property

Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

### Osservazioni

Se il valore non è specificato, viene utilizzato il filtro predefinito che rimuove le attività non visibili -- cioè le attività discendenti di attività collassate.

### Esempi

Mostra come utilizzare un filtro personalizzato per le attività durante il salvataggio di un file MS Project.

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

        // imposta un filtro per le attività per saltare le attività 'Task5' e 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // vediamo il formato di salvataggio
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // salva il progetto come immagine
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Esempio di filtro personalizzato per le attività che può essere usato durante il salvataggio di un file MS Project (ad esempio) in formato PDF.
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

### Vedi anche

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1)
* class [Task](../../../aspose.tasks/task)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
