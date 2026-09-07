---
title: "OutlineMask.OutlineMask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής OutlineMask. Αρχικοποιεί μια νέα παρουσία της κλάσης OutlineMask"
type: docs
weight: 10
url: /el/net/aspose.tasks/outlinemask/outlinemask/
---
## OutlineMask constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`OutlineMask`](../).

```csharp
public OutlineMask()
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


