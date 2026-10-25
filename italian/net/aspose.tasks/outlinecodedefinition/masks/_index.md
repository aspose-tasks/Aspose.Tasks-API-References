---
title: "OutlineCodeDefinition.Masks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "OutlineCodeDefinition proprietà. Ottiene l'oggetto OutlineMaskCollection. La tabella delle voci che definiscono la maschera del codice di contorno. Istanza OutlineMaskCollection di sola lettura"
type: docs
weight: 100
url: /it/net/aspose.tasks/outlinecodedefinition/masks/
---
## OutlineCodeDefinition.Masks property

Ottiene l'oggetto OutlineMaskCollection. La tabella delle voci che definiscono la maschera del codice di contorno. Istanza [`OutlineMaskCollection`](../../outlinemaskcollection/) di sola lettura.

```csharp
public OutlineMaskCollection Masks { get; }
```

## Esempi

Mostra come lavorare con le definizioni dei codici di struttura.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// crea una nuova definizione di codice di struttura
var outline = new OutlineCodeDefinition();

// imposta il numero del campo di un codice di struttura
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// imposta il nome di un codice di struttura personalizzato
outline.FieldName = "Outline Code1";

// imposta il GUID di un codice di struttura
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// imposta un valore che indica se i valori specificati in questo campo del codice di struttura devono essere valori foglia
outline.LeafOnly = false;

// imposta l'alias di un codice di struttura personalizzato
outline.Alias = "My Outline Code";

// imposta la pronuncia fonetica dell'alias del codice di struttura personalizzato
outline.PhoneticAlias = "Outline Code";

// imposta un valore che indica se i nuovi codici devono avere tutti i livelli. Non disponibile per i Codici Enterprise.
outline.AllLevelsRequired = true;

// imposta un valore che indica se un codice di struttura personalizzato è un codice di struttura personalizzato enterprise
outline.Enterprise = false;

// imposta un riferimento a un altro campo personalizzato per il quale questa definizione di codice di struttura è un alias
outline.EnterpriseOutlineCodeAlias = 0;

// aggiungi una maschera di struttura
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// imposta un valore che indica se i valori specificati devono provenire dalla tabella dei valori
outline.OnlyTableValuesAllowed = false;

// imposta un valore che indica se il codice di struttura personalizzato può essere utilizzato
// dal wizard di sostituzione risorse in Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// imposta un valore che indica se le rientranze di questo codice di struttura devono essere visualizzate.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Vedi anche

* class [OutlineMaskCollection](../../outlinemaskcollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


