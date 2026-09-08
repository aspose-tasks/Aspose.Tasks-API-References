---
title: "Tsk.HyperlinkAddress"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La dirección de un hipervínculo asociado a una tarea"
type: docs
weight: 500
url: /es/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

La dirección de un hipervínculo asociado a una tarea.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Observaciones

La dirección completa (Hipervínculo Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

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


