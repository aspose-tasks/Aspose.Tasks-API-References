---
title: "Tsk.SubprojectName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La ubicación de origen de un subproyecto"
type: docs
weight: 1070
url: /es/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

La ubicación de origen de un subproyecto.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Ejemplos

Muestra cómo crear una tarea de subproyecto.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Agregar tarea
var task = project.RootTask.Children.Add("Task 1");

// Configurando nuevo enlace de subproyecto
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


