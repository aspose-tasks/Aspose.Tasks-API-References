---
title: "Resource.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Resource. Retourne une valeur de code de hachage pour l'instance de la classe Resource"
type: docs
weight: 840
url: /fr/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une ressource.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// le code de hachage d'une ressource est égal à l'UID de la ressource 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Voir aussi

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


