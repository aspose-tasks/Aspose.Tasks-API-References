---
title: "Classe OutlineMaskCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OutlineMaskCollection. Représente une collection d'objets OutlineMask"
type: docs
weight: 1200
url: /fr/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Représente une collection d'objets [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Détermine l'index de l'élément spécifié dans cette collection. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Insère l'élément spécifié à l'index spécifié. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Supprime un élément à l'index spécifié. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


