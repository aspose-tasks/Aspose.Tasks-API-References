---
title: "SimpleSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Ceci est une classe de base abstraite qui permet à l'utilisateur de spécifier des options de base lors de l'enregistrement d'un projet dans un format particulier."
type: docs
weight: 277
url: /fr/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Ceci est une classe de base abstraite qui permet à l'utilisateur de spécifier des options de base lors de l'enregistrement d'un projet dans un format particulier.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [getTasksComparer()](#getTasksComparer--) | Obtient le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [getTasksFilter()](#getTasksFilter--) | Obtient la condition utilisée pour filtrer les tâches affichées sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Définit la condition utilisée pour filtrer les tâches affichées sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Obtient le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé.

**Returns:**
int - le [SaveFileFormat](../../com.aspose.tasks/savefileformat) dans lequel le document sera enregistré.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Obtient le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Obtient la condition utilisée pour filtrer les tâches affichées sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches.

--------------------

Si la valeur n'est pas spécifiée, le filtre par défaut est utilisé, ce qui supprime les tâches non visibles — c.-à-d. les tâches descendantes des tâches réduites.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Définit la condition utilisée pour filtrer les tâches affichées sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches.

--------------------

Si la valeur n'est pas spécifiée, le filtre par défaut est utilisé, ce qui supprime les tâches non visibles — c.-à-d. les tâches descendantes des tâches réduites.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | la condition qui est utilisée pour filtrer les tâches affichées sur les graphiques Gantt, Feuille de tâches et Utilisation des tâches. |

