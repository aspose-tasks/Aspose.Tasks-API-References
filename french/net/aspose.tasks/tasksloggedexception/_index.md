---
title: "Classe TasksLoggedException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TasksLoggedException. Représente le type d'exception interne standard"
type: docs
weight: 2530
url: /fr/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Représente le type d'exception interne standard.

```csharp
public class TasksLoggedException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


