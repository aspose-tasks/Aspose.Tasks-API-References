---
title: "Prj.CriticalSlackLimit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni"
type: docs
weight: 140
url: /it/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


