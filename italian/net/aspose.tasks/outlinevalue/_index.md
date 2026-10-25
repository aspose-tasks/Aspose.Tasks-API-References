---
title: "Classe OutlineValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.OutlineValue class. Rappresenta un valore di outline"
type: docs
weight: 1210
url: /it/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Rappresenta un valore di contorno.

```csharp
public class OutlineValue
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OutlineValue](outlinevalue/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Ottiene o imposta la descrizione di un valore di outline. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Ottiene o imposta la durata se il Tipo è Durata. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Ottiene o imposta un valore che indica se il valore di outline è compresso o meno. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Ottiene o imposta l'Id di un nodo genitore di un codice outline. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Ottiene o imposta il tipo di codice outline. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Ottiene o imposta il valore effettivo. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Ottiene o imposta l'Id univoco di un valore di codice outline all'interno di un progetto. |

## Esempi

Mostra come lavorare con i valori outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// crea un valore outline
var value = new OutlineValue();

// imposta il valore effettivo
value.Value = "Text value 1";

// imposta l'Id univoco di un valore di codice outline all'interno di un progetto
value.ValueId = 1;

// ottieni un GUID che identifica questo valore tra gli altri nell'intero progetto
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// imposta il tipo di codice outline
value.Type = OutlineValueType.Text;

// imposta la descrizione di un valore outline
value.Description = "Text value descr 1";

// imposta un valore che indica se il valore outline è collassato o meno
value.IsCollapsed = false;

// verifica l'Id del valore padre
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// crea un valore outline con durata
var value2 = new OutlineValue();

// imposta il valore della durata
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// imposta l'Id univoco di un valore di codice outline all'interno di un progetto
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


