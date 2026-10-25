---
title: "Project.Set"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project methode. Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container"
type: docs
weight: 1240
url: /nl/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Prj`](../../prj/) voor het ophalen van de eigenschapssleutel. |
| waarde | de waarde. |

## Voorbeelden

Toont hoe de attributen van een taak ingesteld kunnen worden.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | Key`2 | de opgegeven eigenschapssleutel. [`Prj`](../../prj/) voor het ophalen van de eigenschapssleutel. |
| waarde | DateTime | de waarde. |

## Voorbeelden

Toont hoe de attributen van een taak ingesteld kunnen worden.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


