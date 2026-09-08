---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De bronlocatie van een subproject"
type: docs
weight: 1070
url: /nl/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

De bronlocatie van een subproject.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Voorbeelden

Toont hoe een subprojecttaak te maken.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Taak toevoegen
var task = project.RootTask.Children.Add("Task 1");

// Instellen van nieuwe subprojectkoppeling
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


