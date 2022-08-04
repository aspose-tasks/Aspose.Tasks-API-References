---
title: Add
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Ajouter la tâche spécifiée à linstance duTaskCollectionaspose.tasks/taskcollectionclass. Si ParentProject.CalculationMode est None lutilisateur doit invoquer Project.Recalculate après avoir utilisé cette méthode il reprogrammera toutes les tâches du projet dates de début/fin définit les dates anticipées/tardives et calculera les champs dépendants tels que les marges le travail et les champs de coût les identifiants et les niveaux hiérarchiques. Si ParentProject.CalculationMode est Manuel la méthode ne calculera automatiquement que lID de la tâche le niveau hiérarchique et les numéros hiérarchiques. Si ParentProject.CalculationMode est Automatique la méthode replanifie automatiquement toutes les tâches du projet début/fin dates définit les dates anticipées/tardives calcule les marges les champs de travail et de coût recalcule les identifiants et les niveaux hiérarchiques.
type: docs
weight: 50
url: /fr/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Ajouter la tâche spécifiée à l'instance du[`TaskCollection`](../../taskcollection)class. Si ParentProject.CalculationMode est None, l'utilisateur doit invoquer Project.Recalculate() après avoir utilisé cette méthode (il reprogrammera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux hiérarchiques). Si ParentProject.CalculationMode est Manuel, la méthode ne calculera automatiquement que l'ID de la tâche, le niveau hiérarchique et les numéros hiérarchiques. Si ParentProject.CalculationMode est Automatique, la méthode replanifie automatiquement toutes les tâches du projet (début/fin dates, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût, recalcule les identifiants et les niveaux hiérarchiques).

```csharp
public void Add(Task item)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| item | Task | la tâche spécifiée qui doit être ajoutée à cette collection de tâches. |

### Voir également

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* espace de noms [Aspose.Tasks](../../taskcollection)
* Assemblée [Aspose.Tasks](../../../)

---

## Add() {#add}

Ajoute une nouvelle tâche à la collection de tâches de projet au même niveau hiérarchique que la dernière tâche.

```csharp
public Task Add()
```

### Return_Value

renvoie l'instance nouvellement ajoutée du[`Task`](../../task) classer.

### Voir également

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* espace de noms [Aspose.Tasks](../../taskcollection)
* Assemblée [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Ajoute une nouvelle tâche à la collection de tâches enfants.

```csharp
public Task Add(string taskName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| taskName | String | le nom de tâche spécifié. |

### Return_Value

renvoie l'instance nouvellement ajoutée du[`Task`](../../task) classer.

### Voir également

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* espace de noms [Aspose.Tasks](../../taskcollection)
* Assemblée [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Ajoute une nouvelle tâche récurrente à la collection de tâches enfants.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| taskName | String | le nom de tâche spécifié. |
| beforeTaskId | Int32 | L'identifiant spécifié d'une tâche avant laquelle une nouvelle tâche sera insérée. |

### Return_Value

renvoie une tâche qui a été insérée avant une tâche avec l'identifiant spécifié.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException est levée si l'ID spécifié n'est pas un ID de tâche valide. |

### Voir également

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* espace de noms [Aspose.Tasks](../../taskcollection)
* Assemblée [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Insère une nouvelle tâche avant une tâche avec l'identifiant spécifié et sur le même niveau hiérarchique.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Les paramètres les paramètres spécifiés pour la création de la tâche récurrente. |

### Return_Value

renvoie l'instance nouvellement ajoutée du[`Task`](../../task) classer.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Levé si les paramètres spécifiés sont nuls. |
| ArgumentException | Levé si les paramètres spécifiés ne sont pas valides. |

### Voir également

* class [Task](../../task)
* class [RecurringTaskParameters](../../recurringtaskparameters)
* class [TaskCollection](../../taskcollection)
* espace de noms [Aspose.Tasks](../../taskcollection)
* Assemblée [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
