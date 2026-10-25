---
title: "Resource.IsRoot"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient le drapeau indiquant si la ressource est une ressource racine. Une ressource racine est une ressource spéciale destinée à prendre en charge les internes des formats MS Projects et n’est pas destinée à être utilisée directement dans le code des utilisateurs."
type: docs
weight: 470
url: /fr/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Obtient le drapeau indiquant si la ressource est une ressource racine. La ressource racine est une ressource spéciale destinée à prendre en charge les internes des formats de MS Project et n'est pas destinée à être utilisée directement dans le code de l'utilisateur.

```csharp
public virtual bool IsRoot { get; }
```

## Exemples

Montre comment utiliser la propriété IsRoot pour ignorer la ressource racine.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Voir aussi

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


