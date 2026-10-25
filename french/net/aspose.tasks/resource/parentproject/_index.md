---
title: "Resource.ParentProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient le projet parent pour ce conteneur"
type: docs
weight: 600
url: /fr/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Obtient le projet parent pour ce conteneur.

```csharp
public Project ParentProject { get; }
```

## Exemples

Montre comment utiliser le projet parent de la ressource.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Définit un travail pour la ressource en utilisant le type d'unité de temps de travail du projet par défaut.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Voir aussi

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


