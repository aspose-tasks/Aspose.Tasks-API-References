---
title: "Tsk.Contact"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le nom d'une personne responsable d'une tâche"
type: docs
weight: 220
url: /fr/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Le nom d'une personne responsable d'une tâche.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


