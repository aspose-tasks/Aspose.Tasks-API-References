---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Helperklasse die nuttige bewerkingen met taken biedt."
type: docs
weight: 307
url: /nl/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Helperklasse die nuttige bewerkingen met taken biedt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Past het opgegeven algoritme toe op elke taak van een boom. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Bouwt een nieuwe boom van taken die aan de voorwaarde voldoen. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Vindt een taak die aan de voorwaarde voldoet in een boom van taken. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Berekent recursief het aantal onderliggende taken van een taak over alle niveaus. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Past het opgegeven algoritme toe op elke taak van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wortel van de boom |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Toegepast algoritme. |
| niveau | int | Niveau van de worteltaak. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Bouwt een nieuwe boom van taken die aan de voorwaarde voldoen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wortel van de boom. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Toegepaste voorwaarde. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Vindt een taak die aan de voorwaarde voldoet in een boom van taken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wortel van de boom. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Toegepaste voorwaarde. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Berekent recursief het aantal onderliggende taken van een taak over alle niveaus.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | De taak waarvan de kinderen worden berekend. |

**Returns:**
int - Het aantal kinderen.
