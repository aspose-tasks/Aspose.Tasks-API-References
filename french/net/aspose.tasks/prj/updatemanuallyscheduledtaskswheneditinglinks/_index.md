---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les tâches manuelles doivent être mises à jour lorsque les liens ont été modifiés"
type: docs
weight: 770
url: /fr/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

Détermine si les tâches manuelles doivent être mises à jour lorsque les liens ont été modifiés.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## Exemples

Montre comment lire/écrire la propriété Prj.UpdateManuallyScheduledTasksWhenEditingLinks.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


