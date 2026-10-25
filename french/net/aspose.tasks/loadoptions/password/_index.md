---
title: "LoadOptions.Password"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété LoadOptions. Obtient ou définit un mot de passe de protection."
type: docs
weight: 50
url: /fr/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Obtient ou définit un mot de passe de protection.

```csharp
public string Password { get; set; }
```

## Exemples

Montre comment charger le projet protégé par mot de passe en utilisant une instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


