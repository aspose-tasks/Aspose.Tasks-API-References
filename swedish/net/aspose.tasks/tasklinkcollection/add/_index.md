---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks för .NET API-referens
description: TaskLinkCollection metod. Returnerar en instans av FinishStartTaskLink som har lagts till i TaskLinkCollectionobjektet.
type: docs
weight: 40
url: /sv/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Returnerar en instans av Finish-Start[`TaskLink`](../../tasklink/) som har lagts till i TaskLinkCollection-objektet.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | Task | Föregående uppgift. |
| succ | Task | Efterföljande uppgift. |

### Returvärde

en uppgiftslänkinstans som har lagts till detta objekt.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | Om någon av inmatningsuppgifterna är lika med null dåArgumentNullException kommer att kastas. |

### Se även

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namnutrymme [Aspose.Tasks](../../tasklinkcollection/)
* hopsättning [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Returnerar en instans av[`TaskLink`](../../tasklink/) som har lagts till i TaskLinkCollection-objektet.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | Task | Föregående uppgift. |
| succ | Task | Efterföljande uppgift. |
| linkType | TaskLinkType | Länktyp[`TaskLinkType`](../../tasklinktype/) |

### Returvärde

en uppgiftslänkinstans som har lagts till detta objekt.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | Om någon av inmatningsuppgifterna är lika med null dåArgumentNullException kommer att kastas. |

### Se även

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namnutrymme [Aspose.Tasks](../../tasklinkcollection/)
* hopsättning [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Returnerar en instans av[`TaskLink`](../../tasklink/) som har lagts till i TaskLinkCollection-objektet.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | Task | Föregående uppgift. |
| succ | Task | Efterföljande uppgift. |
| linkType | TaskLinkType | Länktyp[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Länklag[`Duration`](../../duration/). |

### Returvärde

en uppgiftslänk som har lagts till detta objekt.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | Om någon av inmatningsuppgifterna är lika med null dåArgumentNullException kommer att kastas. |

### Se även

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namnutrymme [Aspose.Tasks](../../tasklinkcollection/)
* hopsättning [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Detta är stubbimplementeringen av ICollections Add-metod, som bara kastar NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | TaskLink | Objektet att lägga till. |

### Se även

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namnutrymme [Aspose.Tasks](../../tasklinkcollection/)
* hopsättning [Aspose.Tasks](../../../)


