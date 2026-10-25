---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Verwijdert de opgegeven taak uit een taakboom."
type: docs
weight: 246
url: /nl/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Verwijdert de opgegeven taak uit een taakboom.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Initialiseert een nieuw exemplaar van de [RemoveTask](../../com.aspose.tasks/removetask) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Doe niets. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Doe niets. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Verwijdert de taak van de opgegeven bovenliggende taak. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Initialiseert een nieuw exemplaar van de [RemoveTask](../../com.aspose.tasks/removetask) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Taak om te verwijderen. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Doe niets.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Doe niets.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Verwijdert de taak van de opgegeven bovenliggende taak.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Bovenliggende taak. |
| niveau | int | Boomknooppuntniveau. |

