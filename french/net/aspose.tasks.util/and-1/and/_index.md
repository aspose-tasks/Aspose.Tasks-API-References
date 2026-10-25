---
title: "And1.And"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur And. Initialise une nouvelle instance de la classe And"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

Initialise une nouvelle instance de la classe [`And`](../).

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cond1 | ICondition`1 | Première condition. |
| cond2 | ICondition`1 | Deuxième condition. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


