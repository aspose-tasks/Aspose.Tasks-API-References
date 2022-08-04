---
title: Task
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Représente une tâche dans un projet.
type: docs
weight: 2060
url: /fr/net/aspose.tasks/task/
---
## Task class

Représente une tâche dans un projet.

```csharp
public class Task : IEquatable<Task>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Obtient une collection d'affectations de ressources pour cet objet. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Obtient ou définit la collection de valeurs de référence de la tâche. |
| [Children](../../aspose.tasks/task/children) { get; } | Obtient une collection de tâches enfant de cet objet. Objet TaskCollection qui représente les tâches enfants. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Obtient l'objet ExtendedAttributeCollection contenant les valeurs d'un attribut étendu. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Obtient ou définit[`OutlineCodeCollection`](../outlinecodecollection) objet. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Obtient le projet parent d'une tâche. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Obtient la tâche parent d'une tâche. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | Obtient un[`TaskCollection`](../taskcollection) objet qui contient tous les prédécesseurs de cet objet Tâche. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Obtient l'instance de[`RecurringTaskInfo`](../recurringtaskinfo) classe pour la tâche qui est une tâche récurrente ; si la tâche n'est pas récurrente, renvoie null ;  Les informations pour l'instance de[`RecurringTaskInfo`](../recurringtaskinfo) est présent uniquement au format de fichier mpp. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Obtient une collection SplitPart qui représente les parties d'une tâche. |
| [Successors](../../aspose.tasks/task/successors) { get; } | Obtient un[`TaskCollection`](../taskcollection) objet qui contient tous les successeurs de cet objet Tâche. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Obtient ou définit un objet TimephasedDataCollection de cette tâche. Le bloc de données chronologique associé à une tâche. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Crée une copie complète d'une tâche sans sous-tâches. |
| [Delete](../../aspose.tasks/task/delete)() | Supprime une tâche de la collection de tâches du projet parent et toutes ses affectations. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Renvoie une valeur indiquant si cette instance est égale à une tâche spécifiée. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Renvoie une valeur de code de hachage pour cette tâche. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | Retours[`TimephasedDataCollection`](../timephaseddatacollection) objet avec[`TimephasedData`](./timephaseddata) valeurs dans les dates de début et de fin données. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | Retours[`TimephasedDataCollection`](../timephaseddatacollection) objet avec[`TimephasedData`](./timephaseddata) valeurs dans les dates de début et de fin données du type de données chronologiques spécifié. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Déplace la tâche actuelle au même niveau hiérarchique avant une tâche avec l'Id. spécifié Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (il replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives) et calcule les champs dépendants tels que les marges, les champs de travail et de coût, les niveaux hiérarchiques). Si ParentProject.CalculationMode est Manuel, la méthode calculera uniquement l'ID de tâche, le niveau hiérarchique et les numéros hiérarchiques automatiquement. Si ParentProject. CalculationMode est Automatique, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates au plus tôt/au plus tard, calcule les marges, les champs de travail et de coût, recalcule les identifiants et les niveaux hiérarchiques). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Déplace la tâche actuelle au même niveau hiérarchique avant la tâche spécifiée. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (il replanifiera toutes les tâches du projet (dates de début/fin, définit tôt/ dates de retard) et calculer les champs dépendants tels que les marges, les champs de travail et de coût, les niveaux hiérarchiques). Si ParentProject.CalculationMode est manuel, la méthode ne calculera automatiquement que l'ID de tâche, le niveau hiérarchique et les numéros hiérarchiques. Si ParentProject.CalculationMode est automatique la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût, recalcule les identifiants et les niveaux hiérarchiques). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Indente une tâche dans le plan. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Promeut une tâche dans le plan. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Collecte de manière récursive toutes les tâches enfants de cette tâche. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| override [ToString](../../aspose.tasks/task/tostring)() | Renvoie la représentation sous forme de chaîne courte d'une tâche. Les détails exacts de la représentation ne sont pas spécifiés et peuvent être modifiés. |

### Remarques

La **Tâche** représente un mandrin atomique de travail.

On peut utiliser **Tâche**pour planifier un projet en créant des tâches et en leur affectant les ressources appropriées. Les tâches d'un projet sont organisées sous la forme d'une arborescence hiérarchique enracinée, avec une tâche racine et des sous-arborescences de tâches enfants.

Pour construire un arbre de tâches, on peut utiliser une collection spécialisée[`TaskCollection`](../taskcollection) en accédant[`RootTask`](../project/roottask) propriété ex:

```csharp
Project project = new Project();

// ajouter de nouvelles tâches
Task task1 = project.RootTask.Children.Add(); // une tâche parent avec un nom vide est ajoutée
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // insère une tâche avant la childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// enregistre le projet dans l'un des formats disponibles
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks)
* Assemblée [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
