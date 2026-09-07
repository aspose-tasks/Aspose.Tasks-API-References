---
title: "Project.Set"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Mappa la proprietà specificata al valore specificato in questo contenitore"
type: docs
weight: 1240
url: /it/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Mappa la proprietà specificata al valore specificato in questo contenitore.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Prj`](../../prj/) per ottenere la chiave della proprietà. |
| val | il valore. |

## Esempi

Mostra come impostare gli attributi dell'attività.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Mappa la proprietà specificata al valore specificato in questo contenitore.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | Key`2 | la chiave della proprietà specificata. [`Prj`](../../prj/) per ottenere la chiave della proprietà. |
| val | DateTime | il valore. |

## Esempi

Mostra come impostare gli attributi dell'attività.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


