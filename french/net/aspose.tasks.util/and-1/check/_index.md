---
title: "And1.Check"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode And. Retourne vrai si l'objet spécifié satisfait les conditions"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/and-1/check/
---
## And&lt;T&gt;.Check method

Renvoie true si l'objet spécifié satisfait les conditions.

```csharp
public bool Check(T el)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | L'objet à vérifier. |

### Valeur de retour

Vrai si l'objet satisfait les conditions.

## Exemples

Montre comment utiliser la condition &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // rassembler toutes les tâches du projet
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crée une condition de filtre qui filtre les tâches de synthèse
    var condition1 = new SummaryCondition();

    // crée une condition de filtre qui filtre les tâches non nulles
    var condition2 = new NotNullCondition();

    // et les joint en appliquant la condition <see cref=\"Aspose.Tasks.Util.And`1\" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // applique la condition aux tâches collectées
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### Voir aussi

* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


