---
title: "Project.SetBaseline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Enregistre les champs de référence dans la référence spécifiée pour l'ensemble du projet"
type: docs
weight: 1250
url: /fr/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Enregistre les champs de base de référence dans la base de référence spécifiée pour l’ensemble du projet.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | Le type de référence dans lequel enregistrer les données de référence. |

## Exemples

Montre comment créer des références pour un projet complet.

```csharp
var project = new Project();

// Ajout de tâches
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Définir la référence pour les tâches spécifiées
project.SetBaseline(BaselineType.Baseline);
```

### Voir aussi

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Enregistre les champs de base de référence dans la base de référence spécifiée pour les tâches sélectionnées.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | Le type de référence dans lequel enregistrer les données de référence. |
| taskCollection | IEnumerable`1 | Liste des tâches pour lesquelles enregistrer les données de référence. |

## Exemples

Montre comment créer des références définies pour des tâches spécifiques.

```csharp
var project = new Project();

// Ajout de tâches
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Définir la référence pour les tâches spécifiées
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Voir aussi

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


