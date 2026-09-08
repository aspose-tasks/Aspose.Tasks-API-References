---
title: "Tsk.Hyperlink"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De titel of verklarende tekst voor een hyperlink die aan een taak is gekoppeld"
type: docs
weight: 490
url: /nl/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

De titel of verklarende tekst voor een hyperlink die aan een taak is gekoppeld.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## Voorbeelden

Toont hoe de Tsk.Hyperlink-eigenschappen gelezen/schreven kunnen worden.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


