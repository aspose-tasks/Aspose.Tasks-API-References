---
title: "Table.TableType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Table. Λαμβάνει ή ορίζει τον τύπο του πίνακα για τον καθορισμένο πίνακα."
type: docs
weight: 100
url: /el/net/aspose.tasks/table/tabletype/
---
## Table.TableType property

Λαμβάνει ή ορίζει τον τύπο πίνακα για τον καθορισμένο πίνακα.

```csharp
public ItemType TableType { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε έναν νέο πίνακα (χρησιμοποιώντας για προβολές).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// λάβετε έναν πίνακα για επεξεργασία
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// ρυθμίστε κάποιες ιδιότητες
// ορίστε μια τιμή που υποδεικνύει αν το ύψος της γραμμής κεφαλίδας του πίνακα μπορεί να προσαρμοστεί
table.AdjustHeaderRowHeight = true;

// ορίστε τη μορφή ημερομηνίας του πίνακα.
table.DateFormat = DateFormat.DateDdMmYyyy;

// ορίστε μια τιμή που υποδεικνύει αν η πρώτη στήλη ενός πίνακα είναι κλειδωμένη ή επεξεργάσιμη
table.LockFirstColumn = true;

// ορίστε το ύψος της γραμμής σε έναν πίνακα, όπου το ύψος της γραμμής είναι ο αριθμός των γραμμών κειμένου
table.RowHeight = 10;

// ορίζει μια τιμή που υποδεικνύει αν θα εμφανιστεί η διεπαφή 'Προσθήκη Νέας Στήλης'
table.ShowAddNewColumn = true;

// ορίστε μια τιμή που υποδεικνύει αν το έργο εμφανίζει το όνομα του πίνακα στη λίστα επιλογής Πίνακες στην καρτέλα Προβολή της κορδέλας
table.ShowInMenu = true;

// επιτρέπει την αποθήκευση του ενημερωμένου πίνακα
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* enum [ItemType](../../itemtype/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


