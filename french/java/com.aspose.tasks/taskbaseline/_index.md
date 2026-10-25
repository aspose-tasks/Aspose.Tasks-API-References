---
title: "TaskBaseline"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente la ligne de base d'une tâche."
type: docs
weight: 291
url: /fr/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Représente la ligne de base d'une tâche.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Initialise une nouvelle instance de la classe [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implémentation de l'interface IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Renvoie une valeur indiquant si cette instance est égale à l'objet TaskBaseline spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getDuration()](#getDuration--) | Obtient la durée planifiée de la tâche lorsque la ligne de base a été enregistrée. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Obtient une valeur indiquant si la durée de la ligne de base de la tâche était estimée. |
| [getFinish()](#getFinish--) | Obtient la date de fin planifiée de la tâche lorsque la ligne de base a été enregistrée. |
| [getFixedCost()](#getFixedCost--) | Obtient un coût fixe de la tâche lorsque la ligne de base a été enregistrée. |
| [getInterim()](#getInterim--) | Obtient une valeur indiquant s'il s'agit d'une ligne de base intermédiaire. |
| [getStart()](#getStart--) | Obtient la date de début planifiée de la tâche lorsque la ligne de base a été enregistrée. |
| [getTimephasedData()](#getTimephasedData--) | Obtient une instance de TimephasedDataCollection pour cet objet. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Définit la durée planifiée de la tâche lorsque la ligne de base a été enregistrée. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Définit une valeur indiquant si la durée de la ligne de base de la tâche était estimée. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Définit la date de fin planifiée de la tâche lorsque la ligne de base a été enregistrée. |
| [setFixedCost(double value)](#setFixedCost-double-) | Définit un coût fixe de la tâche lorsque la ligne de base a été enregistrée. |
| [setInterim(boolean value)](#setInterim-boolean-) | Définit une valeur indiquant si c’est une ligne de base intermédiaire. |
| [setStart(Date value)](#setStart-java.util.Date-) | Définit la date de début prévue de la tâche lorsque la ligne de base a été enregistrée. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Définit une instance de TimephasedDataCollection pour cet objet. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Initialise une nouvelle instance de la classe [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tâche parente de la ligne de base. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | l'objet Baseline spécifié avec lequel comparer cette instance. |

**Returns:**
int - renvoie -1 si cette instance est inférieure à l'objet spécifié, 1 si cette instance est supérieure à l'objet spécifié ; sinon renvoie 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Renvoie une valeur indiquant si cette instance est égale à l'objet TaskBaseline spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

**Returns:**
booléen - renvoie true si cette instance est égale à l’objet TaskBaseline spécifié ; sinon, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet à comparer avec cette instance. |

**Returns:**
booléen - **True** si l’objet spécifié est un TaskBaseline qui possède la même valeur UID que cette instance ; sinon, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtient la durée planifiée de la tâche lorsque la ligne de base a été enregistrée.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Obtient une valeur indiquant si la durée de la ligne de base de la tâche était estimée.

**Returns:**
booléen - une valeur indiquant si la durée de la ligne de base de la tâche était estimée.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtient la date de fin planifiée de la tâche lorsque la ligne de base a été enregistrée.

**Returns:**
java.util.Date - la date de fin prévue de la tâche lorsque la ligne de base a été enregistrée.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Obtient un coût fixe de la tâche lorsque la ligne de base a été enregistrée.

**Returns:**
double - un coût fixe de la tâche lorsque la ligne de base a été enregistrée.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Obtient une valeur indiquant s'il s'agit d'une ligne de base intermédiaire.

**Returns:**
booléen - une valeur indiquant si c’est une ligne de base intermédiaire.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtient la date de début planifiée de la tâche lorsque la ligne de base a été enregistrée.

**Returns:**
java.util.Date - la date de début prévue de la tâche lorsque la ligne de base a été enregistrée.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtient une instance de TimephasedDataCollection pour cet objet. Les données temporelles associées à la ligne de base de la tâche.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Définit la durée planifiée de la tâche lorsque la ligne de base a été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durée prévue de la tâche lorsque la ligne de base a été enregistrée. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Définit une valeur indiquant si la durée de la ligne de base de la tâche était estimée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la durée de la ligne de base de la tâche était estimée. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Définit la date de fin planifiée de la tâche lorsque la ligne de base a été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de fin prévue de la tâche lorsque la ligne de base a été enregistrée. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Définit un coût fixe de la tâche lorsque la ligne de base a été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un coût fixe de la tâche lorsque la ligne de base a été enregistrée. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Définit une valeur indiquant si c’est une ligne de base intermédiaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si c’est une ligne de base intermédiaire. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Définit la date de début prévue de la tâche lorsque la ligne de base a été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de début prévue de la tâche lorsque la ligne de base a été enregistrée. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Définit une instance de TimephasedDataCollection pour cet objet. Les données temporelles associées à la ligne de base de la tâche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | une instance de TimephasedDataCollection pour cet objet. |

