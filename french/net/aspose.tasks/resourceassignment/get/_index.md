---
title: "ResourceAssignment.Get"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ResourceAssignment méthode. Retourne la valeur à laquelle la propriété est mappée dans ce conteneur"
type: docs
weight: 700
url: /fr/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Asn`](../../asn/) pour obtenir la clé de propriété. |

### Valeur de retour

la valeur à laquelle la propriété est mappée dans ce conteneur.

## Exemples

Montre comment créer une affectation et obtenir/definir les propriétés d'affectation communes.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


