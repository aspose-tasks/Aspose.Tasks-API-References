---
title: "Classe TasksLoggedException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TasksLoggedException. Rappresenta il tipo di eccezione interno standard"
type: docs
weight: 2530
url: /it/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Rappresenta il tipo di eccezione interno standard.

```csharp
public class TasksLoggedException : ApplicationException
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Ottiene le informazioni di registrazione dell'eccezione. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Ottiene le informazioni sull'operazione dell'eccezione. |

## Esempi

Mostra come leggere il testo del log e il tipo di eccezione per verificare i problemi con l'esportazione MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // esporta il progetto come file MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


