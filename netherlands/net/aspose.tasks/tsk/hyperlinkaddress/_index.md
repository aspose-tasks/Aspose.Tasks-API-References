---
title: "Tsk.HyperlinkAddress"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Het adres voor een hyperlink gekoppeld aan een taak"
type: docs
weight: 500
url: /nl/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

Het adres voor een hyperlink die aan een taak is gekoppeld.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Opmerkingen

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

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


