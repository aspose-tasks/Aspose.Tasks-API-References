---
title: "Classe OutlineMaskCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineMaskCollection. Rappresenta una collezione di oggetti OutlineMask"
type: docs
weight: 1200
url: /it/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Rappresenta una collezione di oggetti [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

## Esempi

Mostra come lavorare con le raccolte di maschere outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// cancella le maschere outline
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

// inserisci una maschera errata
outline.Masks.Insert(0, maskWrong);

// modifica la maschera usando l'accesso per indice della raccolta
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// rimuovi una maschera errata per indice
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// itera sulle maschere
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

### Vedi anche

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


