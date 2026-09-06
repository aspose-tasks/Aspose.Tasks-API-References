---
title: "Not1.Check"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Not. Retourne true si l'objet spécifié satisfait la condition"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Renvoie true si l'objet spécifié satisfait la condition.

```csharp
public bool Check(T el)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | L'objet à vérifier. |

### Valeur de retour

Vrai si l'objet satisfait la condition.

## Exemples

Montre comment utiliser la condition &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // rassembler toutes les tâches du projet
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crée une condition de filtre
    var filter = new NullCondition();

    // et l'inverse en appliquant la condition <see cref=\"Aspose.Tasks.Util.Not`1\" />
    var condition = new Not<Task>(filter);

    // applique la condition aux tâches collectées
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

        // travaillez avec d'autres propriétés...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Voir aussi

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


