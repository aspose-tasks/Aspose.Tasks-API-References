---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SimpleSaveOptions-Eigenschaft. Gibt die Bedingung zurück oder legt sie fest, die zum Filtern von Aufgaben verwendet wird, die im Gantt-Aufgabenblatt- und Aufgaben-Nutzungs-Diagramm dargestellt werden."
type: docs
weight: 30
url: /de/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Liest oder setzt die Bedingung, die verwendet wird, um Aufgaben, die im Gantt‑, Task‑Sheet‑ und Task‑Usage‑Diagramm gerendert werden, zu filtern.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Hinweise

Wenn kein Wert angegeben ist, wird der Standardfilter verwendet, der nicht sichtbare Aufgaben entfernt – d. h. Nachfolgeraufgaben von zusammengeklappten Aufgaben.

## Beispiele

Zeigt, wie ein benutzerdefinierter Aufgabenfilter beim Speichern einer MS-Project-Datei verwendet wird.

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

        // Setze einen Aufgabenfilter, um die Aufgaben 'Task5' und 'Task3' zu überspringen.
        TasksFilter = new CustomTasksFilter()
    };

    // Lass uns das Speicherformat prüfen
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // Projekt als Bild speichern
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Beispiel für einen benutzerdefinierten Aufgabenfilter, der beim Speichern einer MS-Project-Datei (z. B.) im PDF-Format verwendet werden kann.
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

### Siehe auch

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


