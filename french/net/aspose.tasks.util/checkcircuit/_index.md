---
title: "Classe CheckCircuit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Util.CheckCircuit. Vérifie un arbre de tâches pour savoir s'il contient un circuit"
type: docs
weight: 2680
url: /fr/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Vérifie si un arbre (de tâches) contient un circuit.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Initialise une nouvelle instance de la classe `CheckCircuit`. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Vérifiez si l'objet spécifié a déjà été traité. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Exemples

Montre comment détecter la structure du projet cassée.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// vérifier la structure du projet.
// Le <see cref="TasksException"> sera levé si la structure du projet est incorrecte.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Voir aussi

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


