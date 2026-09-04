---
title: "TaskLink"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un lien de prédécesseur."
type: docs
weight: 295
url: /fr/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Représente un lien de prédécesseur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getCrossProjectName()](#getCrossProjectName--) | Obtient le projet prédécesseur externe. |
| [getLagFormat()](#getLagFormat--) | Obtient le format d’expression du retard. |
| [getLinkLag()](#getLinkLag--) | Obtient le retard en dixièmes de minute ou en pourcentage. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Obtient la durée du retard, selon le LagFormat. |
| [getLinkType()](#getLinkType--) | Obtient le type d’un lien. |
| [getPredTask()](#getPredTask--) | Obtient la tâche prédécesseur. |
| [getSuccTask()](#getSuccTask--) | Obtient la tâche successeur. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l’instance de la classe [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Obtient une valeur indiquant si un prédécesseur fait partie d’un autre projet. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Définit une valeur indiquant si un prédécesseur fait partie d’un autre projet. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Définit le projet prédécesseur externe. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Définit le format d’expression du retard. |
| [setLinkLag(int value)](#setLinkLag-int-) | Définit le retard en dixièmes de minute ou en pourcentage. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Définit la durée du retard, selon le LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Définit le type d’un lien. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Définit la tâche prédécesseur. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Définit la tâche successeur. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne d’un TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | L’instance spécifiée de la classe [TaskLink](../../com.aspose.tasks/tasklink) à comparer avec cette instance. |

**Returns:**
booléen - **True** si l’instance spécifiée de la classe [TaskLink](../../com.aspose.tasks/tasklink) a les mêmes tâches prédécesseur et successeur que cette instance ; sinon, **false**.
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
boolean - **True** si l'objet spécifié est un TaskLink qui a le même prédécesseur et successeur que cette instance ; sinon, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Obtient le projet prédécesseur externe.

**Returns:**
java.lang.String - le projet prédécesseur externe.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Obtient le format d’expression du retard.

**Returns:**
byte - le format d'expression du retard.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Obtient le retard en dixièmes de minute ou en pourcentage.

**Returns:**
int - le retard en dixièmes de minute ou en pourcentage.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Obtient la durée du retard, selon le LagFormat.

**Returns:**
double - durée du retard, selon le LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Obtient le type d’un lien.

**Returns:**
int - le type d'un lien.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Obtient la tâche prédécesseur.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Obtient la tâche successeur.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l’instance de la classe [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Obtient une valeur indiquant si un prédécesseur fait partie d’un autre projet.

**Returns:**
boolean - une valeur indiquant si un prédécesseur fait partie d'un autre projet.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Définit une valeur indiquant si un prédécesseur fait partie d’un autre projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si un prédécesseur fait partie d'un autre projet. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Définit le projet prédécesseur externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le projet prédécesseur externe. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Définit le format d’expression du retard.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte | le format d'expression du retard. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Définit le retard en dixièmes de minute ou en pourcentage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le retard en dixièmes de minute ou en pourcentage. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Définit la durée du retard, selon le LagFormat.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | durée du retard, selon le LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Définit le type d’un lien.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type d'un lien. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Définit la tâche prédécesseur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tâche prédécesseur. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Définit la tâche successeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tâche successeur. |

### toString() {#toString--}
```
public String toString()
```


Renvoie la représentation sous forme de chaîne d'un TaskLink. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

**Returns:**
java.lang.String - chaîne qui représente l'objet TaskLink.
