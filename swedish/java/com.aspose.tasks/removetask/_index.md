---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tar bort den angivna uppgiften från en uppgiftsträd."
type: docs
weight: 246
url: /sv/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Tar bort den angivna uppgiften från en uppgiftsträd.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Initialiserar en ny instans av klassen [RemoveTask](../../com.aspose/tasks/removetask). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Gör ingenting. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Gör ingenting. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Tar bort uppgiften från den angivna föräldrauppgiften. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Initialiserar en ny instans av klassen [RemoveTask](../../com.aspose/tasks/removetask).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Uppgift att ta bort. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Gör ingenting.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objekt att bearbeta. |
| nivå | int | Trädnodnivå. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Gör ingenting.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objekt att bearbeta. |
| nivå | int | Trädnodnivå. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Tar bort uppgiften från den angivna föräldrauppgiften.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Föräldrauppgift. |
| nivå | int | Trädnodnivå. |

