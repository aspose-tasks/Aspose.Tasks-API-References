---
title: "Classe TaskValidationException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskValidationException. Représente une exception qui est levée lorsque des erreurs sont trouvées dans les tâches de projets après recalcul"
type: docs
weight: 2510
url: /fr/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Représente une exception qui est levée lorsque des erreurs sont détectées dans les tâches du projet après recalcul.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Obtient la tâche qui a causé l'exception. |

## Exemples

Montre dans quelles conditions l'exception &lt;see cref="TaskValidationException" /&gt; peut être levée.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // définir accidentellement des dates incorrectes
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // exécuter le recalcul du projet avec un indicateur pour exécuter la validation   
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Voir aussi

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


