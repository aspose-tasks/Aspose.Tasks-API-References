---
title: "TasksLoggedException.LogText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TasksLoggedException. Obtient les informations de journalisation de l'exception"
type: docs
weight: 10
url: /fr/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

Obtient les informations de journalisation de l'exception.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


