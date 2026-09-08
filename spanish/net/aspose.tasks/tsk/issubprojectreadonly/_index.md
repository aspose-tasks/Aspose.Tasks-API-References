---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si un subproyecto es de solo lectura"
type: docs
weight: 710
url: /es/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

Determina si un subproyecto es de solo lectura.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsSubprojectReadOnly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


