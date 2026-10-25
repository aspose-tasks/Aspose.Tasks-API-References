---
title: "Tsk.Hyperlink"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El título o texto explicativo de un hipervínculo asociado a una tarea"
type: docs
weight: 490
url: /es/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

El título o texto explicativo de un hipervínculo asociado a una tarea.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## Ejemplos

Muestra cómo leer/escribir las propiedades Tsk.Hyperlink.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


