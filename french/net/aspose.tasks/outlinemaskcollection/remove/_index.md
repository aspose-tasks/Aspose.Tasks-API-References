---
title: "OutlineMaskCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineMaskCollection method. Supprime la première occurrence d'un objet spécifique de cette collection"
type: docs
weight: 110
url: /fr/net/aspose.tasks/outlinemaskcollection/remove/
---
## OutlineMaskCollection.Remove method

Supprime la première occurrence d'un objet spécifique de cette collection.

```csharp
public bool Remove(OutlineMask item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | OutlineMask | l'objet spécifié à supprimer. |

### Valeur de retour

true si l'objet spécifié a été supprimé avec succès de cette collection ; sinon, false.

## Exemples

Montre comment travailler avec des collections de masques de contour.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// effacer les masques de contour
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// insérer un masque incorrect
outline.Masks.Insert(0, maskWrong);

// modifier le masque en utilisant l'accès par index de la collection
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// supprimer un masque incorrect par index
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// itérer sur les masques
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### Voir aussi

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


