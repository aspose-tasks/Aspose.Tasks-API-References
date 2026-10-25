---
title: "TaskUtils.Find"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUtils. Trouve une tâche qui satisfait la condition dans un arbre de tâches"
type: docs
weight: 30
url: /fr/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Trouve une tâche qui satisfait la condition dans un arbre de tâches.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| root | Tâche | Racine de l'arbre. |
| cond | ICondition`1 | Condition appliquée. |

### Valeur de retour

Tâche si la tâche a été trouvée, sinon null.

## Exemples

Montre comment utiliser &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.Find\" /&gt; méthode.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // construit un nouvel arbre de tâches qui satisfont la condition 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Retourne vrai si l'objet spécifié satisfait les conditions.
    /// </summary>
    /// <param name=\"el\">L'objet à vérifier.</param>
    /// <returns>Vrai si l'objet satisfait les conditions.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Voir aussi

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


