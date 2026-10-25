---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "SimpleSaveOptions proprietà. Ottiene o imposta il formato in cui il documento verrà salvato se questo oggetto di opzioni di salvataggio viene utilizzato"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio.

```csharp
public SaveFileFormat SaveFormat { get; }
```

## Esempi

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

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


