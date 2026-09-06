---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraReadOptions. Obtient ou définit un indicateur qui spécifie si les identifiants uniques originaux des entités doivent être conservés"
type: docs
weight: 20
url: /fr/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Obtient ou définit un indicateur qui spécifie si les identifiants uniques originaux des entités doivent être conservés.

```csharp
public bool PreserveUids { get; set; }
```

## Exemples

Montre comment charger un projet Primavera avec l'Id spécifié en utilisant &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// définir les options de lecture Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// travailler avec le projet...
```

### Voir aussi

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


