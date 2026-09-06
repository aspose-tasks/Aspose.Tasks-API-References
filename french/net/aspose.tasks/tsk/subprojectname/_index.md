---
title: "Tsk.SubprojectName"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L'emplacement source d'un sous-projet"
type: docs
weight: 1070
url: /fr/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

L'emplacement source d'un sous-projet.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Exemples

Montre comment créer une tâche de sous-projet.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Ajouter une tâche
var task = project.RootTask.Children.Add("Task 1");

// Définition du nouveau lien de sous‑projet
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


