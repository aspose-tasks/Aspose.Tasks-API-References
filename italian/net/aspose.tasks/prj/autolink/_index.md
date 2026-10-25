---
title: "Prj.Autolink"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se i compiti inseriti o spostati sono collegati automaticamente"
type: docs
weight: 70
url: /it/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Determina se le attività inserite o spostate sono collegate automaticamente.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


