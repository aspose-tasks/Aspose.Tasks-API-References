---
title: "Classe InvalidPasswordException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.InvalidPasswordException. Rappresenta il tipo di eccezione che viene lanciata quando si apre un file protetto da password con una password errata."
type: docs
weight: 910
url: /it/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Rappresenta il tipo di eccezione che viene lanciata quando si apre un file protetto da password con una password errata.

```csharp
public class InvalidPasswordException : TasksException
```

## Esempi

Mostra come gestire &lt;see cref=\"InvalidPasswordException\"/&gt; durante la lettura di file di progetto protetti da password.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // lavorare con il progetto ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // il messaggio è "Il progetto è protetto da password. La password non è fornita o è errata."
    Console.WriteLine(e.Message);
}
```

### Vedi anche

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


