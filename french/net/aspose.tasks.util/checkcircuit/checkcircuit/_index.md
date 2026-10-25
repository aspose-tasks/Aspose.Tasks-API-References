---
title: "CheckCircuit.CheckCircuit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur de CheckCircuit. Initialise une nouvelle instance de la classe CheckCircuit"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Initialise une nouvelle instance de la classe [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


