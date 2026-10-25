---
title: "Classe MPPSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.MPPSaveOptions. Consente di specificare opzioni aggiuntive quando si salvano i dati del progetto in MPP"
type: docs
weight: 2050
url: /it/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Consente di specificare opzioni aggiuntive durante il salvataggio dei dati del progetto in MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Inizializza una nuova istanza della classe `MPPSaveOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Ottiene o imposta un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Ottiene o imposta una password utilizzata per proteggere il file MPP risultante. Attualmente è supportata per i formati MS Project 2010 e versioni successive. Un valore null indica che il file di progetto non è protetto. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Ottiene o imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP. MS Project crea un'assegnazione di risorsa vuota per ogni attività. Imposta questo flag su true per rimuoverle al salvataggio. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Ottiene o imposta un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP. I dati dei filtri includono le collezioni Project.TaskFilters e Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Ottiene o imposta un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP. I dati dei gruppi includono le collezioni Project.TaskGroups e Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Ottiene o imposta un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. Attualmente è supportata la scrittura di VbaModule.SourceCode. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Ottiene o imposta un valore che indica se scrivere i dati della visualizzazione durante il salvataggio di un progetto in formato MPP. I dati della visualizzazione includono le collezioni Project.Views, Filters e Tables. |

## Esempi

Mostra come salvare il progetto in uno stream come file MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // crea opzioni di salvataggio
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP
        RemoveInvalidAssignments = true
    };

    // salva MPP con opzioni
    project.Save(stream, options);
}
```

### Vedi anche

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


