---
title: Tsk.HyperlinkAddress
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The address for a hyperlink associated with a task
type: docs
weight: 500
url: /net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

The address for a hyperlink associated with a task.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Remarks

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

## Examples

Shows how to read/write Tsk.Hyperlink properties.

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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


