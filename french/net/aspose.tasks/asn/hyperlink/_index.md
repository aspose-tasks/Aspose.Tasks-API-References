---
title: "Asn.Hyperlink"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le titre ou le texte explicatif d'un hyperlien associé à une affectation"
type: docs
weight: 280
url: /fr/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

Le titre ou le texte explicatif d'un hyperlien associé à une affectation.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

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


