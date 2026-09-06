---
title: "Tsk.HyperlinkSubAddress"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L'emplacement spécifique dans un document d'un hyperlien associé à une tâche"
type: docs
weight: 510
url: /fr/net/aspose.tasks/tsk/hyperlinksubaddress/
---
## Tsk.HyperlinkSubAddress field

L'emplacement spécifique dans un document d'un hyperlien associé à une tâche.

```csharp
public static readonly Key<string, TaskKey> HyperlinkSubAddress;
```

## Remarques

L’adresse complète (Hyperlink Href dans Microsoft Project) de l’hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

## Exemples

Montre comment lire/écrire les propriétés Tsk.Hyperlink.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


