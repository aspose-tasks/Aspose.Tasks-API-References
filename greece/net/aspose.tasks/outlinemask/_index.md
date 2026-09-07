---
title: "Κλάση OutlineMask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.OutlineMask. Αναπαριστά τέσσερα στοιχεία μιας μάσκας που ορίζει τη μορφή κώδικα περιγράμματος"
type: docs
weight: 1190
url: /el/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Αντιπροσωπεύει τέσσερα στοιχεία μιας μάσκας που ορίζει τη μορφή κώδικα περίγραμμα.

```csharp
public class OutlineMask
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [OutlineMask](outlinemask/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `OutlineMask`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Λαμβάνει ή ορίζει το μέγιστο μήκος (σε χαρακτήρες) των τιμών του κώδικα περιγράμματος. 0 εάν το μήκος δεν ορίζεται. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Λαμβάνει ή ορίζει το επίπεδο μιας μάσκας. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Λαμβάνει ή ορίζει το διαχωριστικό των τιμών κώδικα. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο μιας μάσκας. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


