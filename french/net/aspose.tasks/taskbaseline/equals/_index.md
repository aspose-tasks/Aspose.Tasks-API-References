---
title: "TaskBaseline.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskBaseline. Retourne une valeur indiquant si cette instance est égale à l'objet TaskBaseline spécifié"
type: docs
weight: 100
url: /fr/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à l’objet `TaskBaseline` spécifié.

```csharp
public bool Equals(TaskBaseline other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | TaskBaseline | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie true si cette instance est égale à l'objet TaskBaseline spécifié ; sinon, false.

## Exemples

Montre comment vérifier l'égalité des baselines.

```csharp
var project = new Project();

// création de TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// afficher la durée de la baseline de la tâche
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// L'égalité des baselines est vérifiée par rapport aux valeurs de la baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Voir aussi

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_2}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet à comparer avec cette instance. |

### Valeur de retour

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des baselines.

```csharp
var project = new Project();

// création de TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// afficher la durée de la baseline de la tâche
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// L'égalité des baselines est vérifiée par rapport aux valeurs de la baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Voir aussi

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


