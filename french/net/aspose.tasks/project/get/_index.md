---
title: "Project.Get"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Retourne la valeur à laquelle la propriété est mappée dans ce conteneur"
type: docs
weight: 1080
url: /fr/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Prj`](../../prj/) pour obtenir la clé de propriété. |

### Valeur de retour

la valeur à laquelle la propriété est mappée dans ce conteneur.

## Exemples

Montre comment vérifier la version d'un projet.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Afficher la version du projet
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


