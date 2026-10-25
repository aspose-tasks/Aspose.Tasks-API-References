---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SimpleSaveOptions-eigenschap. Haalt de voorwaarde op of stelt deze in die wordt gebruikt om taken te filteren die worden weergegeven op het Gantt‑taakblad en de taakgebruik‑grafieken"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Opmerkingen

Als de waarde niet is opgegeven, wordt de standaardfilter gebruikt die niet‑zichtbare taken verwijdert — d.w.z. onderliggende taken van samengevouwen taken.

## Voorbeelden

Toont hoe je een aangepaste takenfilter gebruikt bij het opslaan van een MS Project-bestand.

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

        // stel een takenfilter in om taak 'Task5' en 'Task3' over te slaan
        TasksFilter = new CustomTasksFilter()
    };

    // laten we het opslagformaat controleren
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // sla het project op als afbeelding
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Voorbeeld van een aangepaste takenfilter die kan worden gebruikt bij het opslaan van een MS Project-bestand (bijvoorbeeld) in PDF-formaat.
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

### Zie ook

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


