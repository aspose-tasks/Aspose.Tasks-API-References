---
title: "Classe OutlineCodeDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineCodeDefinition. Rappresenta una definizione di codice di struttura."
type: docs
weight: 1170
url: /it/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Rappresenta una definizione di codice di contorno.

```csharp
public sealed class OutlineCodeDefinition
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | Inizializza una nuova istanza della classe `OutlineCodeDefinition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Ottiene o imposta l'alias di un codice di struttura personalizzato. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Ottiene o imposta un valore che indica se i nuovi codici devono avere tutti i livelli. Non disponibile per i Codici Enterprise. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Ottiene o imposta un valore che indica se un codice di struttura personalizzato è un codice di struttura personalizzato enterprise. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Ottiene o imposta un riferimento a un altro campo personalizzato per il quale questa definizione di codice di struttura è un alias. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Ottiene o imposta il numero di campo di un codice di struttura. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Ottiene o imposta il nome di un codice di struttura personalizzato. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Ottiene o imposta il GUID di un codice di struttura. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Ottiene o imposta un valore che indica se i valori specificati in questo campo di codice di struttura devono essere valori foglia. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | Ottiene l'oggetto OutlineMaskCollection. La tabella delle voci che definiscono la maschera del codice di struttura. Istanza di sola lettura [`OutlineMaskCollection`](../outlinemaskcollection/). |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Ottiene o imposta un valore che indica se i valori specificati devono provenire dalla tabella dei valori. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Ottiene o imposta la pronuncia fonetica dell'alias del codice di struttura personalizzato. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Ottiene o imposta un valore che indica se il codice di struttura personalizzato può essere utilizzato dalla procedura guidata di sostituzione risorse in Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Ottiene o imposta un valore che indica se le rientranze di questo codice di struttura devono essere visualizzate. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | Ottiene l'oggetto OutlineValueCollection. I valori della tabella associata a questo codice di struttura. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


