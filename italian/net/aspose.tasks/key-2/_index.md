---
title: "Struttura KeyTK"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Struttura Aspose.Tasks.Key2TK. Rappresenta una chiave di proprietà di una classe del tipo specificato. Un'istanza di questa classe è utilizzata quando si ottiene o si imposta una proprietà di un contenitore"
type: docs
weight: 930
url: /it/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Rappresenta una chiave di proprietà di una classe del tipo specificato. Un'istanza di questa classe viene utilizzata quando si ottiene o si imposta la proprietà di un contenitore.

```csharp
public struct Key<T, K>
    where K : struct
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo del valore della proprietà. |
| K | Il tipo della chiave della proprietà. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Ottiene la chiave della proprietà. |

## Esempi

Mostra come leggere/scrivere la proprietà Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


