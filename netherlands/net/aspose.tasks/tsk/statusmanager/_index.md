---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De naam van de bedrijfsresource die statusupdates voor de huidige taak van resources moet ontvangen"
type: docs
weight: 1050
url: /nl/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

De naam van de bedrijfsresource die statusupdates voor de huidige taak van resources moet ontvangen.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.StatusManager gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


