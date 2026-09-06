---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "LoadOptions propriété. Obtient ou définit une instance spécifiée de la classe PrimaveraReadOptions qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera Primavera P6 XER ou Primavera P6 Xml"
type: docs
weight: 60
url: /fr/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Obtient ou définit une instance spécifiée de la classe [`PrimaveraReadOptions`](../../primaverareadoptions/) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


