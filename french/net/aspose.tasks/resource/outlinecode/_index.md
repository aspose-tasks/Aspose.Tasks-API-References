---
title: "Resource.OutlineCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient un objet OutlineCodeCollection. La valeur d'un code de plan"
type: docs
weight: 540
url: /fr/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Obtient un objet OutlineCodeCollection. La valeur d'un code de contour.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Remarques

Deux éléments de données sont nécessaires - un pointeur vers la table des codes de plan spécifiée par le FieldID, et la valeur spécifiée soit par le ValueID soit par le pointeur ValueGUID vers la liste des valeurs.

## Exemples

Montre comment travailler avec les valeurs de plan de ressource.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### Voir aussi

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


