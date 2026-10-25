---
title: "Task.OutlineCodes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient ou définit l'objet OutlineCodeCollection"
type: docs
weight: 880
url: /fr/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Obtient ou définit l'objet [`OutlineCodeCollection`](../../outlinecodecollection/) .

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Remarques

Deux éléments de données sont nécessaires - un pointeur vers la table des codes de plan spécifiée par le FieldID, et la valeur spécifiée soit par le ValueID soit par le pointeur ValueGUID vers la liste des valeurs.

## Exemples

Montrez comment lire les valeurs du code de plan du task.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### Voir aussi

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


