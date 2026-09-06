---
title: "Classe TasksWritingException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TasksWritingException. Représente le type d'exception d'écriture interne standard"
type: docs
weight: 2560
url: /fr/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Représente le type d'exception interne d'écriture standard.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Propriétés

| Nom | Description |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Obtient les informations de journalisation de l'exception. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Obtient les informations d'opération de l'exception. |

## Exemples

Montre comment lire le texte du journal et le type d'exception pour vérifier les problèmes avec l'exportation MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // exporter le projet en tant que fichier MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Voir aussi

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


