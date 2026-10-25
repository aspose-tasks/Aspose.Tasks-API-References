---
title: "Tsk.Hyperlink"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il titolo o il testo esplicativo per un collegamento ipertestuale associato a un'attività"
type: docs
weight: 490
url: /it/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

Il titolo o il testo esplicativo per un collegamento ipertestuale associato a un'attività.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## Esempi

Mostra come leggere/scrivere le proprietà Tsk.Hyperlink.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


