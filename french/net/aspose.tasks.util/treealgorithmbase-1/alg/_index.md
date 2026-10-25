---
title: "TreeAlgorithmBase1.Alg"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TreeAlgorithmBase. Traite un nœud d'un arbre."
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/treealgorithmbase-1/alg/
---
## TreeAlgorithmBase&lt;T&gt;.Alg method

Traite un nœud d'un arbre.

```csharp
public abstract void Alg(T el, int level)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


