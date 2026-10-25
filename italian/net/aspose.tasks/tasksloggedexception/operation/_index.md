---
title: "TasksLoggedException.Operation"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TasksLoggedException. Ottiene le informazioni sull'operazione dell'eccezione"
type: docs
weight: 20
url: /it/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Ottiene le informazioni sull'operazione dell'eccezione.

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


