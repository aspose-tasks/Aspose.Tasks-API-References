---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak actief is. Inactieve taken hebben geen invloed meer op andere taken of het algehele projectschema"
type: docs
weight: 550
url: /nl/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Bepaalt of een taak actief is. Inactieve taken hebben geen invloed meer op andere taken of het algehele projectschema.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsActive te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


