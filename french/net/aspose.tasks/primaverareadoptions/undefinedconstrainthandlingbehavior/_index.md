---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraReadOptions. Spécifie le comportement utilisé pour traiter les tâches avec des contraintes indéfinies lues à partir du format XER"
type: docs
weight: 50
url: /fr/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Spécifie le comportement utilisé pour traiter les tâches avec des contraintes indéfinies lues à partir du format XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


