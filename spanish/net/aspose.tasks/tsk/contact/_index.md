---
title: "Tsk.Contact"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El nombre de la persona responsable de una tarea"
type: docs
weight: 220
url: /es/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

El nombre de una persona responsable de una tarea.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


