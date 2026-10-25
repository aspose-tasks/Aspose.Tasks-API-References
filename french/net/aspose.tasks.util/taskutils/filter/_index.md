---
title: "TaskUtils.Filter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUtils. Construit un nouvel arbre de tâches qui satisfont la condition"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Construit un nouvel arbre de tâches qui satisfont la condition.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| root | Tâche | Racine de l'arbre. |
| cond | ICondition`1 | Condition appliquée. |

### Valeur de retour

Racine d'un nouvel arbre.

## Exemples

Montre comment travailler avec une condition.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // construit un nouvel arbre de tâches qui satisfont la condition 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // récupérer des tâches d'un arbre
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // itérer sur une liste simple de tâches 
    // dont les durées sont supérieures ou égales à 2 jours ouvrés
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Retourne vrai si l'objet spécifié satisfait les conditions.
    /// </summary>
    /// <param name=\"el\">L'objet à vérifier.</param>
    /// <returns>Vrai si l'objet satisfait les conditions.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Voir aussi

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


