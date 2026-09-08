---
title: "Tsk.Contact"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De naam van een persoon die verantwoordelijk is voor een taak."
type: docs
weight: 220
url: /nl/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

De naam van een persoon die verantwoordelijk is voor een taak.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.Contact te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


