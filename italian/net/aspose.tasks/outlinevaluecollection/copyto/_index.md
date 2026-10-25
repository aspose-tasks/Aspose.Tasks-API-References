---
title: "OutlineValueCollection.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "OutlineValueCollection metodo. Copia gli elementi di questa collezione nell'array specificato iniziando dall'indice dell'array specificato"
type: docs
weight: 70
url: /it/net/aspose.tasks/outlinevaluecollection/copyto/
---
## OutlineValueCollection.CopyTo method

Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato.

```csharp
public void CopyTo(OutlineValue[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | OutlineValue[] | l'array monodimensionale specificato a cui copiare gli elementi |
| arrayIndex | Int32 | l'indice basato su zero dell'array specificato al quale inizia la copia. |

## Esempi

Mostra come lavorare con le collezioni di valori outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// cancella le collezioni di valori
foreach (var outlineCode in project.OutlineCodes)
{
    // cancella le maschere outline
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

// aggiorna il valore tramite accesso per indice
codeDefinition.Values[0].Value = "654321";

// itera sui valori outline
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// lavora con i valori outline
// ...

// rimuovi un valore quando necessario
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// inserisci un valore nella posizione iniziale
codeDefinition.Values.Insert(0, value);

// verifica la posizione del valore inserito
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// lavora con i valori outline
// ...

// rimuovi l'ultimo valore dalla collezione
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// si può creare un'altra definizione di codice outline
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// e poi copiare i valori outline
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Vedi anche

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


