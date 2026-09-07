---
title: "OutlineMask.Level"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα OutlineMask. Λαμβάνει ή ορίζει το επίπεδο μιας μάσκας"
type: docs
weight: 30
url: /el/net/aspose.tasks/outlinemask/level/
---
## OutlineMask.Level property

Λαμβάνει ή ορίζει το επίπεδο μιας μάσκας.

```csharp
public int Level { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μάσκες περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// ορίστε τον τύπο μιας μάσκας
mask.Type = MaskType.Characters;

// ορίστε το διαχωριστικό των τιμών κώδικα
mask.Separator = "/";

// ορίστε το επίπεδο μιας μάσκας
mask.Level = 1;

// ορίστε το μέγιστο μήκος (σε χαρακτήρες) των τιμών κώδικα περιγράμματος. 0 εάν το μήκος δεν ορίζεται.
mask.Length = 2;

// προσθέστε τη μάσκα στον ορισμό
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Δείτε επίσης

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


