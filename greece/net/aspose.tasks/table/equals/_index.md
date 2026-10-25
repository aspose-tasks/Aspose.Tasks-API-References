---
title: "Table.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Table. Επιστρέφει μια τιμή που υποδεικνύει αν αυτή η περίπτωση είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 120
url: /el/net/aspose.tasks/table/equals/
---
## Table.Equals method

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα του πίνακα.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Η ισότητα των πινάκων ελέγχεται σε σχέση με το UID του πίνακα.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Δείτε επίσης

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


