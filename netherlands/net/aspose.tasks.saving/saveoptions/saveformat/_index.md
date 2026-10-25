---
title: "SaveFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt."
type: docs
weight: 160
url: /nl/net/aspose.tasks.saving/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt.

```csharp
public SaveFileFormat SaveFormat { get; }
```

### Voorbeelden

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

* enum [SaveFileFormat](../../savefileformat)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
