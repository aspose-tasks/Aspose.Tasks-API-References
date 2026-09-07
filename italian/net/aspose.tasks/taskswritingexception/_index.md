---
title: "Classe TasksWritingException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TasksWritingException. Rappresenta il tipo standard di eccezione interna di scrittura"
type: docs
weight: 2560
url: /it/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Rappresenta il tipo di eccezione interno di scrittura standard.

```csharp
public class TasksWritingException : TasksLoggedException
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

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


