---
title: "TaskLinkCollection.Add"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskLinkCollection. Retourne une instance de FinishStart TaskLink qui a été ajoutée à l'objet TaskLinkCollection"
type: docs
weight: 40
url: /fr/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Renvoie une instance de Finish-Start [`TaskLink`](../../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pred | Tâche | Tâche prédécesseur. |
| succ | Tâche | Tâche successeur. |

### Valeur de retour

une instance de lien de tâche qui a été ajoutée à cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Si l'une des tâches d'entrée est égale à null, alors une ArgumentNullException sera levée. |

## Exemples

Montre comment travailler avec des collections de liens de tâche.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// obtenir les tâches
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// lier les tâches
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// imprimer les liens entre les tâches
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifier le lien par accès indexé
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// supprimer tous les liens de tâche
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Voir aussi

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Renvoie une instance de [`TaskLink`](../../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pred | Tâche | Tâche prédécesseur. |
| succ | Tâche | Tâche successeur. |
| linkType | TaskLinkType | Type de lien [`TaskLinkType`](../../tasklinktype/) |

### Valeur de retour

une instance de lien de tâche qui a été ajoutée à cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Si l'une des tâches d'entrée est égale à null, alors une ArgumentNullException sera levée. |

## Exemples

Montre comment travailler avec des collections de liens de tâche.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// obtenir les tâches
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// lier les tâches
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// imprimer les liens entre les tâches
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifier le lien par accès indexé
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// supprimer tous les liens de tâche
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Voir aussi

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Renvoie une instance de [`TaskLink`](../../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pred | Tâche | Tâche prédécesseur. |
| succ | Tâche | Tâche successeur. |
| linkType | TaskLinkType | Type de lien [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Délai du lien [`Duration`](../../duration/). |

### Valeur de retour

un lien de tâche qui a été ajouté à cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Si l'une des tâches d'entrée est égale à null, alors une ArgumentNullException sera levée. |

## Exemples

Montre comment travailler avec des collections de liens de tâche.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// obtenir les tâches
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// lier les tâches
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// imprimer les liens entre les tâches
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifier le lien par accès indexé
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// supprimer tous les liens de tâche
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Voir aussi

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | TaskLink | L'élément à ajouter. |

### Voir aussi

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


