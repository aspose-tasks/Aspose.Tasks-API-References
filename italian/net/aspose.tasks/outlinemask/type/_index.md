---
title: "OutlineMask.Type"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà OutlineMask. Ottiene o imposta il tipo di una maschera"
type: docs
weight: 50
url: /it/net/aspose.tasks/outlinemask/type/
---
## OutlineMask.Type property

Ottiene o imposta il tipo di una maschera.

```csharp
public MaskType Type { get; set; }
```

## Esempi

Mostra come lavorare con le maschere di contorno.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// imposta il tipo di una maschera
mask.Type = MaskType.Characters;

// imposta il separatore dei valori di codice
mask.Separator = "/";

// imposta il livello di una maschera
mask.Level = 1;

// imposta la lunghezza massima (in caratteri) dei valori di codice di contorno. 0 se la lunghezza non è definita.
mask.Length = 2;

// aggiungi la maschera alla definizione
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Vedi anche

* enum [MaskType](../../masktype/)
* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


