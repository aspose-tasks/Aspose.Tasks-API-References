---
title: "Tsk.StatusManager"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le nom de la ressource d'entreprise qui doit recevoir les mises à jour de statut pour la tâche en cours provenant des ressources"
type: docs
weight: 1050
url: /fr/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Le nom de la ressource d'entreprise qui doit recevoir les mises à jour d'état pour la tâche actuelle provenant des ressources.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


