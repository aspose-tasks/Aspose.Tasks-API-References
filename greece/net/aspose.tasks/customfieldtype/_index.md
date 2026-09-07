---
title: "Απαρίθμηση CustomFieldType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.CustomFieldType. Καθορίζει τον τύπο ενός προσαρμοσμένου πεδίου"
type: docs
weight: 380
url: /el/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Καθορίζει τον τύπο ενός προσαρμοσμένου πεδίου.

```csharp
public enum CustomFieldType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Null | `0` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Null. |
| Cost | `1` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Κόστους. |
| Date | `2` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Ημερομηνίας. |
| Duration | `3` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Διάρκειας. |
| Finish | `4` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Ολοκλήρωσης. |
| Flag | `5` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Σημαίας. |
| Number | `6` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Αριθμού. |
| Start | `7` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Έναρξης. |
| Text | `8` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Κειμένου. |
| OutlineCode | `9` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου Κώδικα Περιγράμματος. |
| RBS | `10` | Υποδεικνύει τύπο προσαρμοσμένου πεδίου RBS (Δομή Διάσπασης Πόρων). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// εργασία με ορισμούς...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


