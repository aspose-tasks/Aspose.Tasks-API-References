---
title: "OutlineValueCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineValueCollection méthode. Supprime un élément à l'index spécifié"
type: docs
weight: 120
url: /fr/net/aspose.tasks/outlinevaluecollection/removeat/
---
## OutlineValueCollection.RemoveAt method

Supprime un élément à l'index spécifié.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index | Int32 | l'index zéro basé spécifié pour supprimer un élément. |

## Exemples

Montre comment travailler avec les collections de valeurs de contour.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// effacer les collections de valeurs
foreach (var outlineCode in project.OutlineCodes)
{
    // effacer les masques de contour
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// mettre à jour la valeur par accès à l'index
codeDefinition.Values[0].Value = "654321";

// itérer sur les valeurs de contour
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// travailler avec les valeurs de contour
// ...

// supprimer une valeur si nécessaire
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// insérer une valeur à la position de départ
codeDefinition.Values.Insert(0, value);

// vérifier la position de la valeur insérée
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// travailler avec les valeurs de contour
// ...

// supprimer la dernière valeur de la collection
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// on peut créer une autre définition de code de contour
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// et ensuite copier les valeurs de contour
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Voir aussi

* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


