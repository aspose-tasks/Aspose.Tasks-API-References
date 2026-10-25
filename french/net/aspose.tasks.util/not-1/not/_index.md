---
title: "Not1.Not"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur Not. Initialise une nouvelle instance de la classe Not"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

Initialise une nouvelle instance de la classe [`Not`](../).

```csharp
public Not(ICondition<T> condition)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| condition | ICondition`1 | Condition spécifiée. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


