---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task methode. Retourneert een hashcode-waarde voor deze Task"
type: docs
weight: 1350
url: /nl/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Retourneert een hashcode-waarde voor deze Task.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe je een hashcode van een taak kunt verkrijgen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// de hashcode van een taak is gebaseerd op de uid en de naam van de taak
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


