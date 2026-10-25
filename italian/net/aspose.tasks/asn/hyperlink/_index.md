---
title: "Asn.Hyperlink"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Il titolo o il testo esplicativo di un collegamento ipertestuale associato a un'assegnazione"
type: docs
weight: 280
url: /it/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

Il titolo o il testo esplicativo di un collegamento ipertestuale associato a un'assegnazione.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## Esempi

Mostra come leggere/scrivere le proprietà del collegamento ipertestuale.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


