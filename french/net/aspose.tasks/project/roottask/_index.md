---
title: "Project.RootTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient la racine de l'arbre des tâches"
type: docs
weight: 800
url: /fr/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Obtient la racine de l'arbre des tâches.

```csharp
public Task RootTask { get; }
```

## Exemples

Montre comment ajouter une tâche dans un projet en utilisant la tâche racine du projet.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


