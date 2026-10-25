---
title: "Table.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Table. Επιστρέφει έναν κωδικό κατακερματισμού για αυτόν τον Table."
type: docs
weight: 130
url: /el/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Επιστρέφει έναν κωδικό κατακερματισμού για αυτόν τον Πίνακα.

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κωδικό κατακερματισμού ενός πίνακα.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Ο κωδικός κατακερματισμού ενός πίνακα είναι ίσος με το UID του πίνακα.
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Δείτε επίσης

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


