---
title: "Asn.HyperlinkAddress"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. L'adresse d'un hyperlien associé à une affectation"
type: docs
weight: 290
url: /fr/net/aspose.tasks/asn/hyperlinkaddress/
---
## Asn.HyperlinkAddress field

L'adresse d'un hyperlien associé à l'affectation.

```csharp
public static readonly Key<string, AsnKey> HyperlinkAddress;
```

## Remarques

L’adresse complète (Hyperlink Href dans Microsoft Project) de l’hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

## Exemples

Montre comment lire/écrire les propriétés d'hyperlien.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


