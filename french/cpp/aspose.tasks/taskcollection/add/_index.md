---
title: "Aspose::Tasks::TaskCollection::Add méthode"
linktitle: "Ajouter"
articleTitle: "Ajouter"
second_title: "Aspose.Tasks pour C++"
description: "Ajoute une nouvelle tâche à la collection de tâches du projet au même niveau de plan que la dernière tâche."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Ajoute une nouvelle tâche à la collection de tâches du projet au même niveau de plan que la dernière tâche.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Insère une nouvelle tâche avant une tâche avec l'identifiant spécifié et au même niveau de hiérarchie.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Paramètre | Description |
| --- | --- |
| paramètres | Les paramètres spécifiés pour la création d'une tâche récurrente. |

---

## Add (3 of 5) {#add_3}

Ajoutez la tâche spécifiée à l'instance de la classe TaskCollection. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (Cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de hiérarchie). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de hiérarchie et les numéros de hiérarchie automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût, recalcule les identifiants et les niveaux de hiérarchie).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Paramètre | Description |
| --- | --- |
| élément | la tâche spécifiée qui doit être ajoutée à cette collection de tâches. |

---

## Add (4 of 5) {#add_4}

Ajoute une nouvelle tâche à la collection des tâches enfants.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Paramètre | Description |
| --- | --- |
| taskName | le nom de la tâche spécifiée. |

---

## Add (5 of 5) {#add_5}

Ajoute une nouvelle tâche récurrente à la collection des tâches enfants.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Paramètre | Description |
| --- | --- |
| taskName | le nom de la tâche spécifiée. |
| beforeTaskId | L'identifiant spécifié d'une tâche avant lequel une nouvelle tâche sera insérée. |

