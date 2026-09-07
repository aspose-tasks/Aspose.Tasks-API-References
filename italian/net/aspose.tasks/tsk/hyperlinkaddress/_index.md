---
title: "Tsk.HyperlinkAddress"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. L'indirizzo per un collegamento ipertestuale associato a un'attività"
type: docs
weight: 500
url: /it/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

L'indirizzo per un collegamento ipertestuale associato a un'attività.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Osservazioni

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

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


