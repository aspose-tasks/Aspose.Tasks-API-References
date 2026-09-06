---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si un projet a été créé par un utilisateur Project Server plutôt que par un utilisateur NT"
type: docs
weight: 460
url: /fr/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Détermine si un projet a été créé par un utilisateur Project Server plutôt que par un utilisateur NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


