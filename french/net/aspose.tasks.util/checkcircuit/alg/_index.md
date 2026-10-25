---
title: "CheckCircuit.Alg"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CheckCircuit. Vérifie si l'objet spécifié a déjà été traité"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Vérifiez si l'objet spécifié a déjà été traité.

```csharp
public override void Alg(Task el, int level)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | Tâche | Objet à traiter. |
| niveau | Int32 | Niveau du nœud d'arbre. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


