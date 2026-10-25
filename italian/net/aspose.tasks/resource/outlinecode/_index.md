---
title: "Resource.OutlineCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene un oggetto OutlineCodeCollection. Il valore di un codice di struttura"
type: docs
weight: 540
url: /it/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Ottiene un oggetto OutlineCodeCollection. Il valore di un codice di contorno.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Osservazioni

Sono necessari due dati - un puntatore alla tabella dei codici di struttura specificata dal FieldID, e il valore specificato o dal puntatore ValueID o ValueGUID all'elenco dei valori.

## Esempi

Mostra come lavorare con i valori di struttura delle risorse.

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

### Vedi anche

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


