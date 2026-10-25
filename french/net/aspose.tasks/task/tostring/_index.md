---
title: "Task.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Retourne une représentation sous forme de chaîne courte d'une tâche. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer."
type: docs
weight: 1420
url: /fr/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Renvoie une représentation courte sous forme de chaîne d'une tâche. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

```csharp
public override string ToString()
```

### Valeur de retour

chaîne courte qui représente l'objet tâche.

## Exemples

Montre comment trier les tâches par nom.

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


