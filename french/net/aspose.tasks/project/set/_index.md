---
title: "Project.Set"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Associe la propriété spécifiée à la valeur spécifiée dans ce conteneur"
type: docs
weight: 1240
url: /fr/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Prj`](../../prj/) pour obtenir la clé de propriété. |
| val | la valeur. |

## Exemples

Montre comment définir les attributs d'une tâche.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| key | Key`2 | la clé de propriété spécifiée. [`Prj`](../../prj/) pour obtenir la clé de propriété. |
| val | DateTime | la valeur. |

## Exemples

Montre comment définir les attributs d'une tâche.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


