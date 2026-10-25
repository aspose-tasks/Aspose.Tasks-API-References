---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SimpleSaveOptions-Eigenschaft. Gibt das Format zurück oder legt es fest, in dem das Dokument gespeichert wird, wenn dieses Save-Options-Objekt verwendet wird."
type: docs
weight: 10
url: /de/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

Liest oder setzt das Format, in dem das Dokument gespeichert wird, wenn dieses Save‑Options‑Objekt verwendet wird.

```csharp
public SaveFileFormat SaveFormat { get; }
```

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

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


