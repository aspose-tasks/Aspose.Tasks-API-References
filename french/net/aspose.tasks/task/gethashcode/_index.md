---
title: "Task.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Retourne une valeur de code de hachage pour cette Task"
type: docs
weight: 1350
url: /fr/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Renvoie une valeur de code de hachage pour cette Task.

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une tâche.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// le code de hachage d'une tâche est basé sur l'uid et le nom de la tâche
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


