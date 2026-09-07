---
title: "OutlineCodeDefinition.Values"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "OutlineCodeDefinition proprietà. Ottiene l'oggetto OutlineValueCollection. I valori della tabella associata a questo codice di contorno"
type: docs
weight: 150
url: /it/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

Ottiene l'oggetto OutlineValueCollection. I valori della tabella associata a questo codice di struttura.

```csharp
public OutlineValueCollection Values { get; }
```

## Esempi

Mostra come creare nuovi codici di contorno.

```csharp
var project = new Project(DataDir + "project.mpp");

// Definisci il codice di contorno e la sua maschera
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// Aggiungi valore di contorno
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// Aggiungi codice di contorno al progetto
project.OutlineCodes.Add(code1);

// Definisci il codice di contorno e la sua maschera
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// Aggiungi valore di contorno
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// Aggiungi codice di contorno al progetto
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


