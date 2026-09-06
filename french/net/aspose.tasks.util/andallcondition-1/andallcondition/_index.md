---
title: "AndAllCondition1.AndAllCondition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur AndAllCondition. Initialise une nouvelle instance de la classe AndAllCondition"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Initialise une nouvelle instance de la classe [`AndAllCondition`](../).

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| conditions | List`1 | La liste des conditions. |

## Exemples

Montre comment utiliser la condition &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // rassembler toutes les tâches du projet
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // crée une condition de filtre qui filtre les tâches non nulles
                             new NotNullCondition(),

                             // crée une condition de filtre qui filtre les tâches de synthèse
                             new SummaryCondition()
                         };

    // et les joindre en appliquant la condition <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // applique la condition aux tâches collectées
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


