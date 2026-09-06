---
title: "Class AndAllConditionT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.AndAllCondition1T class. Applique un ET logique à toutes les conditions. Par exemple cond1 AND cond2 AND cond3."
type: docs
weight: 2660
url: /fr/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Applique le ET logique à toutes les conditions. Par exemple : cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'interface de méthode. |

## Constructeurs

| Nom | Description |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Initialise une nouvelle instance de la classe `AndAllCondition`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Renvoie true si l'objet spécifié satisfait les conditions. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


