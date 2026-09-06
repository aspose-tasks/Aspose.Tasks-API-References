---
title: "Classe NotT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.Not1T classe. Applique le NOT logique à la condition spécifiée"
type: docs
weight: 2750
url: /fr/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Applique le NON logique à la condition spécifiée.

```csharp
public class Not<T> : ICondition<T>
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'interface de méthode. |

## Constructeurs

| Nom | Description |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Initialise une nouvelle instance de la classe `Not`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Renvoie true si l'objet spécifié satisfait la condition. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


